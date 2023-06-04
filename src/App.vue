<script>
import AppHeader from './components/AppHeader.vue'
import AppFooter from './components/AppFooter.vue'
import AppMain from './components/AppMain.vue'
import AppBanner from './components/AppBanner.vue'
import AppUnderFooter from './components/AppUnderFooter.vue'

export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter,
    AppBanner,
    AppUnderFooter
  }
}

</script>

<template>
  <AppHeader />
  <AppMain />
  <AppBanner/>
  <AppFooter />
  <AppUnderFooter />
</template>

<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;
</style>