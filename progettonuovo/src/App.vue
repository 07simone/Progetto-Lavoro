<template>
  <div id="app">
    <IndexHeader />
    <main>
      <IndexJumbotron />
      <HomePage />
    </main>
    
    <indexMain />
    <IndexFooter/>
  </div>
</template>

<script>
import IndexHeader from './components/indexHeader.vue'
import IndexJumbotron from './components/indexJumbotron.vue'
import IndexFooter from './components/indexFooter.vue'
import indexMain from './components/indexMain.vue'
import HomePage from './pages/HomePage.vue'
export default {
  name: 'App',
  components: {
    IndexHeader,
    IndexJumbotron,
    indexMain,
    IndexFooter,
    HomePage
}
}
</script>

<style lang="scss">
@import "./style/main-style.scss";
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
