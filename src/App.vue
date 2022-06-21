<template>
  <div id="app">
    <Header :name="선제"></Header>
    <LoginHome/>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import Header from './components/Header.vue';
import LoginHome from './components/LoginHome.vue'


@Options({
  components: {
    Header,
    LoginHome
  }
})
export default class App extends Vue {
  name: string = '안녕하세요.';
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
