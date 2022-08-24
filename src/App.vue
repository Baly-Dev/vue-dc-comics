<template>
  <div id="app">
    <!-- templates -->
    <AppHeader />
  </div>
</template>



<script>
import AppHeader from './components/AppHeader.vue';

export default {
  name: 'App',
  components: {
    AppHeader
}
}
</script>

<style lang="scss">

  @import './src/styles/global.scss'

</style>
