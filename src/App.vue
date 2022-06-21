<template>
  <div id="app">
    <Header :name="username"></Header>
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
      username: ''
    }
  },
  methods: {
      deliverName(value: string) {
        console.log("deliverName");
        console.log('dasda' + this.username);

        this.username = value;
        
      }
  }
})
export default class App extends Vue {
  username!: string;
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
