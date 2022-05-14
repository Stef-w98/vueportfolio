<template>
  <nav>
    <h1>Stef Wouters</h1>
    <div class="links">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
      <img id="icon" src="./assets/moon.png" alt="Light/Dark Mode">
    </div>
  </nav>
  <router-view/>
</template>

<style lang="scss">
:root{
  --primary-color: #edf2fc;
  --secondary-color: #212121;
}
.darktheme{
  --primary-color: #000106;
  --secondary-color: #fff;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background-color: var(--primary-color);
  color: var(--secondary-color);
}
body{
  margin: 0;
  background-color: var(--primary-color);
}
.links{
  display: flex;
  align-items: center;
  text-align: center;
}
.links img{
  margin: 0 3rem 0 2rem;
  width: 30px;
  cursor: pointer;
}
nav {
  display: flex;
  justify-content: space-between;
  text-align: center;
  padding: 1.2rem;

  h1{
    color: var(--secondary-color);
    margin: 0;
  }
  a {
    font-size: 18px;
    color: var(--secondary-color);
    padding: 0.4rem;
    text-decoration: none;

    &.router-link-exact-active {
      color: var(--secondary-color);
    }
  }
}
</style>
