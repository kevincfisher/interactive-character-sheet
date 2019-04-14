<template>
  <div id="app">
    <Wrapper>
        <CharacterSheet/>
    </Wrapper>
  </div>
</template>

<script>
import Wrapper from './components/Wrapper.vue'
import CharacterSheet from './components/CharacterSheet.vue'
export default {
  name: 'app',
  components: {
    Wrapper,
    CharacterSheet
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
}
</style>
