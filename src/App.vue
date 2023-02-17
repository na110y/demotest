<template>
  <div id="App">
    <theHeader></theHeader>
    <router-view></router-view>
    <theFooter></theFooter>
  </div>
</template>
<script>
import theHeader from './components/header/theHeader.vue'
// import TheContent from "./components/content/theContent.vue";
import theFooter from './components/footer/theFooter.vue'
export default {
  name: 'my-app',
  components: {
    theHeader,
    theFooter
  }
}
</script>
<style lang="scss" scoped></style>
