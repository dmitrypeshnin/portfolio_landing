<template>
  <div id="app">
    <Header />
    <PresentationBlock />
    <AboutMeBlock />
  </div>
</template>

<script>
import Header from "@/components/Header";
import PresentationBlock from "@/components/PresentationBlock";
import AboutMeBlock from "@/components/AboutMeBlock";

export default {
  name: 'App',
  components: {
    AboutMeBlock,
    PresentationBlock,
    Header,
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
