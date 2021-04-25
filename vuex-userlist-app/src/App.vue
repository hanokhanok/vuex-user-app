<template>
  <div id="app">
    <div id="nav">
      <div class="menu">
      <router-link to="/">Home</router-link>
      <router-link to="/list">List</router-link>
      </div>
    </div>
    <div id="view">
    <router-view/>
    </div>
  </div>
</template>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

#app {
  width: 100%;
  height: 100vh;
  position: relative;
  background-color: rgb(255, 255, 254);
}

#nav {
  width: 100%;
  height: 60px;
  background-color: rgb(59, 59, 221);
  position: absolute;
  top: 0;
  display: flex;
  align-items: center;
  justify-content: space-around;
}

.menu {
  width: 30%;
  height: 100%;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: space-around;
}
.menu a {color: #fff; font-weight: bold; text-decoration: none;}

#view {
  width: 100%;
  height: calc(100vh - 60px);
  position: absolute;
  top: 60px;
}

</style>
