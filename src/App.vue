<template>
<app-header></app-header>
<app-navigator></app-navigator>
  <router-view/>
</template>

<style lang="scss">

</style>
<script lang="ts">
import AppHeader from './components/shared/Header.vue';
import AppNavigator from './components/shared/Navigator.vue';
export default {
  components: {
    AppHeader,
    AppNavigator
  }
}
</script>
