<script>
import appHeader from './components/appHeader.vue';
import appBg from './components/appBg.vue';
import appMain from './components/appMain.vue';
import appFooter from './components/appFooter.vue'

export default{
  name: 'app',
    components: {
      appHeader,
      appBg,
      appMain,
      appFooter
    }
}
</script>

<template>
  <appHeader/>
  <appBg/>
  <appMain/>
  <appFooter/>
</template>

<style lang="scss">
  @use '../node_modules/bootstrap/scss/bootstrap.scss' as *;
  @use './style/general.scss' as *; 
  @use './style/partials/mixins' as *;
</style>