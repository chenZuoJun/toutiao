<template>
  <div id="app">
    <Header></Header>
    <Nav></Nav>
  </div>
</template>
<script>
 import Header from './components/header.vue'
 import Nav from "./components/navigation"

export default {
 components: {
    Header,
    Nav
  }
}
</script>
<style lang = "less">
body,html,section,div,h1,h2,h3,h4,h5,h6{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

</style>
