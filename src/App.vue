<template>
  <HeaderBlock />
  <UserInput />
</template>


<script>
import HeaderBlock from './components/HeaderBlock.vue'
import UserInput from './components/UserInput.vue';

export default {
  name: 'App',
  components: {
    HeaderBlock,
    UserInput
  }
}

</script>

<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: 'Quicksand', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background: radial-gradient(#303b37, #1a1f1d);
  color: #e1eeeb;
  min-height: 100vh;
}
</style>