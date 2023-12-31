
<script>
import HelloWorld from './components/HelloWorld.vue'
export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data() {
    return {
      data: [],
      url: 'url',
    };
  },
  methods: {
    async getData() {
      try {
        const response = await this.$http.get(this.url);
        this.data = response.data;
      } catch(error) {
        console.log(error);
      }
    },
    async postData(dataToSend) {
      try {
        const postResponse = await this.$http.post('your_post_endpoint', dataToSend);
        console.log('Post response:', postResponse);

      } catch(error) {
        console.error('Error posting data:', error);
      }
    },
  },
  mounted() {
    this.getData();
    this.postData();
  },
};
</script>
<template>
  <div>
    <HelloWorld>
    </HelloWorld>
  </div>
</template>
