<template>
  <div id="app">
    <Header :name="username"></Header>
    <span v-bind:style="style">안녕</span>
    <LoginHome v-on:showName="deliverName"></LoginHome>
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
  },
  data() {
    return {
      username: '',
      text: '',
      style: 'color: white'
    }
  },
  methods: {
      deliverName(value: string) {
        this.username = value;
        this.text = '안녕'
        this.style = 'color: green; font-size: 72px'
      }
  }
})
export default class App extends Vue {
  username!: string;
  text!: string;
  style!: string;
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
