<template>
  <fixed-header>
    <div class="navbar">
      <ul>
        <li>
          <router-link to="/">
            <h3>Home</h3>
          </router-link>
        </li>
        <li>
          <router-link to="/about">
            <h3>About</h3>
          </router-link>
        </li>
        <li>
          <a class="fgoTransparency" href="#/comunicaciones">
            <h3>Benefits List</h3>
          </a>
        </li>
        <li>
          <a class="fgoTransparency" href="#/sorteos">
            <h3>Raffles</h3>
          </a>
        </li>
      </ul>
    </div>
  </fixed-header>
</template>

<script>
  import FixedHeader from 'vue-fixed-header'

  export default {
    components: {
      FixedHeader
    }
  }
</script>

<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
  margin: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
</style>
