<template>
    <main class="container">
        <div class="color-container">
            <ColorComponent v-for="(color, index) in store.colors" :key="index" :color="color" />
        </div>
        <div class="box">

        </div>
    </main>
</template>

<script>
import { store } from '../store.js';
import ColorComponent from './ColorComponent.vue';
export default {
    name: "MainComponent",
    components: {
        ColorComponent
    },
    data() {
        return {
            store
        }
    }
}
</script>

<style lang="scss" scoped>
.color-container {
    display: flex;
    justify-content: space-between;
    margin: 0 20px;
}
</style>