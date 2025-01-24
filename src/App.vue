<template>
 
  <div>
    <h1>Hello {{ name }}</h1>
    <h2>My age is {{ age }}</h2>
    <h2>My gender is Male: {{ isMale }}</h2>
      <h2>My height is {{ height }} even it is not true</h2>
      <h2>My favorite color is {{ colors }}</h2>
      <h2>1 +  1 = {{ age - 9 }}</h2>
      <h2>{{shadowquote[0]}} {{shadowquote[1]}} {{shadowquote[2]}}</h2>
      <div v-text="shadowquote"></div>
      <div v-html="shadowquote[0]"></div>
      <div v-html="msg"></div>
      <div v-html="bomb"></div>
  </div>
</template>

<script>


export default {
  name: 'App',
  data() {
    return {
      name: 'Spoderman',
      age: 11,
      isMale: true,
      height: 43.5,
      colors: ["red", "blue", "yellow"],
      shadowquote: ["<u>I</u>", "am", "atomic"],
      msg: "<a href='https://en.wikipedia.org/wiki/Jeff_the_Land_Shark'>Jeff the shark</a>",
      bomb: "<a onclick='alert(\"boom\")'>boom</a>"
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
