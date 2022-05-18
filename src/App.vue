<template>
  <div id="app">
    <AppPrefooter />
  </div>
</template>

<script>
import AppPrefooter from "./components/AppPrefooter.vue" 

export default {
  name: 'App',
  components: {
    AppPrefooter
  }
}
</script>

<style lang="scss">
@import "./style/common.scss";

</style>
