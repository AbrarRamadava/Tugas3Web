<script>
import Kalkulator from './components/Kalkulator.vue';

export default {
  name: 'App',
  components: {
    Kalkulator,
  },
};
</script>

<template>
  <div id="app">
    <Kalkulator />
  </div>
</template>


<style>
#app {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  font-family: Arial, sans-serif;
}
</style>
