<template>
  <div id="app">
    
    <IndexHeader />

      <IndexJumbotron />
    <main>
      <IndexMain />
    </main>
    <IndexFooter/>
  </div>
</template>

<script>
import IndexHeader from './components/indexHeader.vue'
import IndexJumbotron from './components/indexJumbotron.vue'
import IndexMain from './components/indexMain.vue'
import IndexFooter from './components/indexFooter.vue'
export default {
  name: 'App',
  components: {
    IndexHeader,
    IndexJumbotron,
    IndexMain,
    IndexFooter
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
