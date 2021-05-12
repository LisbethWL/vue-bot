<template>
<header>
  <nav class="nav nav-bar">

      <li class="nav-item">
        <router-link :to="{ name: 'Home' }" exact>
          <img class="logo" src="./assets/build-a-bot-logo.png" />
          Build-a-Bot
        </router-link>
      </li>

      <router-link :to="{ name: 'Build' }" exact>Build</router-link>

  </nav>
</header>
  <main>

    <router-view />
  </main>
</template>

<script>
export default {
  name: 'App',
};
</script>

<style>
  body {
  background: linear-gradient(to bottom, #555, #999);
  background-attachment: fixed;
}
</style>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;

}
main {
  margin: 0 auto;
  padding: 30px;
  background-color: white;
  width: 1024px;
  min-height: 300px;
}
header {
  background-color: #999;
  width: 100%;
  margin: 0px 20px 20px 0px;
}
ul {
  padding: 13px;
  display: flex;
}
.nav-item {
  display: inline-block;
  padding: 5px 10px;
  font-size: 22px;
  border-right: 1px solid #bbb;
  color: white;
}
.nav-bar a {
  font-weight: bold;
  color: white;
  text-decoration: none;
  padding: 10px;
}
.nav-bar a:hover {
  color: pink;
}
.logo {
  vertical-align: middle;
  height: 30px;
}
</style>
