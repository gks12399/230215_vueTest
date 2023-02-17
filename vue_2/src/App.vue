<template>
 <div>
  <!-- 상단 링크 -->
  <nav>
    <!-- router-link to=< >는 index.js의 routes에 있는 path: < >와 같아야 한다. -->
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/databinding/String">String</router-link> |
    <router-link to="/databinding/html">html</router-link> |
    <router-link to="/databinding/input">input</router-link> |
    <router-link to="/databinding/Select">Select</router-link> |
    <router-link to="/databinding/CheckBox">Check</router-link> |
    <router-link to="/databinding/radio">Radio</router-link> |
    <router-link to="/databinding/attr">Attr</router-link> |
    <router-link to="/databinding/list">List</router-link> |
    <router-link to="/databinding/class">Class</router-link> |
    <router-link to="/databinding/style">Style</router-link>
  </nav>
    <router-view/>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
