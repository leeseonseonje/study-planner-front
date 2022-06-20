<template>
  <div>
    <LoginHome/>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import LoginHome from './components/LoginHome.vue'


@Options({
  components: {
    LoginHome
  },
})
export default class Login extends Vue {}
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
