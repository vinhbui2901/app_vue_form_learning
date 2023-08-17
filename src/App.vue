<template>
 <app-form/>
</template>

<script>
import AppForm from './components/app_form/AppForm.vue'


export default {
  name: 'App',
  components: {
    AppForm,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
