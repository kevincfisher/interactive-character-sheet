<template>
    <div id="wrapper" class="wrapper">
        <NavBar/>
        <slot/>
    </div>
</template>

<script>
import NavBar from './NavBar.vue';
export default {
    name: 'Wrapper',
    components: {
        NavBar
    }
}
</script>

<style scoped>
    #wrapper {
        margin: auto;
    }
</style>