<template>
  <v-app>
    <div id="nav">
      <TheNavBar/>
    </div>
    <router-view/>
    <v-toolbar app>
      <v-toolbar-title class="headline text-uppercase">
        <span>Vuetify</span>
        <span class="font-weight-light">MATERIAL DESIGN</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn
        flat
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
      >
        <span class="mr-2">Latest Release</span>
      </v-btn>
    </v-toolbar>

    <v-content>
      <HelloWorld/>
    </v-content>
  </v-app>
</template>

<script>
  import HelloWorld from './components/HelloWorld'
  import TheNavBar from './components/TheNavBar'

  export default {
    name: 'App',
    components: {
      HelloWorld,
      TheNavBar
    },
    data () {
      return {
        //
      }
    }
  }
</script>

<style lang="scss">
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }
  #nav {
    padding: 30px;
    a {
      font-weight: bold;
      color: #2c3e50;
      cursor: pointer;
      text-decoration: none;
      &.router-link-exact-active {
        color: #42b983;
      }
    }
  }
</style>