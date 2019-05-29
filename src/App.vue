<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link>|
      <router-link to="/about">About</router-link>
    </div>-->
    <div class="container">
      <router-view/>
    </div>
  </div>
</template>

<style>
html,
body {
  height: 100%;
}
.container {
  padding: 20px;
  height: 100%;
}

#app {
  height: 100%;
}
</style>
