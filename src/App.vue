<template>
  <HeaderComponent />
  <MainComponent />
</template>

<script>
import { store } from './store.js';
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
export default {
  name: 'App',
  data() {
    return {
      store
    }
  },
  components: {
    HeaderComponent,
    MainComponent
  }
}
</script>

<style lang="scss" scoped></style>