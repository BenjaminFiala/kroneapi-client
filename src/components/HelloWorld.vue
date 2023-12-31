<template>
  <div class="main-container">
    <h1>Krone LLM Textshortening</h1>
    <div class="content">
      <div class="box">
        <textarea class="textbox input-textbox" placeholder="Enter text here" rows="6"></textarea>
        <a class="convert" onclick="App.getData()">Convert</a>
        <textarea class="textbox output-textbox" placeholder="Result" rows="6" readonly></textarea>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld'
}
</script>

<style scoped>

.main-container {
  font-family: Arial, sans-serif;
  color: #333;
  background-color: #f8f8f8;
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
  max-width: 600px;
  margin: 0 auto;
}

h1 {
  margin: 20px 0;
  color: #d32f2f;
}


.content {
  display: flex;
  justify-content: center;
  margin-top: 20px;
}

.box {
  display: flex;
  align-items: center;
  margin: auto;
}


.textbox {
  width: 300px;
  margin: 0 10px;
  padding: 8px;
  border: 1px solid #d32f2f;
  border-radius: 4px;
  font-size: 14px;
  resize: vertical;
}

.input-textbox {
  height: 160px;
}

.output-textbox {
  height: 160px;
  background-color: #ffebee;
}
.convert {
  padding: 8px 12px;
  background-color: #d32f2f;
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  text-decoration: none;
  font-size: 14px;
  transition: background-color 0.3s ease;
}

.convert:hover {
  background-color: #b71c1c;
}
</style>
