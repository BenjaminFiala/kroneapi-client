<template>
  <div>
    <h1>Welcome to KroneAPI</h1>
  <HelloWorld>

  </HelloWorld>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
export default {
  name: 'App',
  components:{HelloWorld},
  data() {
    return {
      data: [],
      apiUrl: 'http://localhost:5000',
    };
  },
  methods: {

  },
  /*mounted() {
    this.getData();
    this.postData();
  },*/
};
</script>
