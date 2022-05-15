<template>
  <nav>
    <div class="navleft">
      <img id="logo" src="assets/faviconwh2.png" alt="SWicon">
      <h1>Stef Wouters</h1>
    </div>
    <div class="links">
      <router-link to="/">Home</router-link>      |
      <router-link to="/about">About</router-link>
      <img id="icon" src="./assets/moon.png" alt="Light/Dark Mode">
    </div>
  </nav>

  <router-view/>

  <footer>
    <div class="footername">
      <p>Stef Wouters</p>
    </div>
    <div class="copyright">
      <p>Copyright © 2022 All Rights Reserved</p>
    </div>
    <div class="socials">
      <img id="iconlnkdn" src="./assets/linkedin.png" alt="linkedin">
      <img id="iconmail" src="./assets/mail.png" alt="mail">
    </div>
  </footer>
</template>

<style lang="scss">
:root {
  --primary-color: #edf2fc;
  --secondary-color: #212121;
}

.darktheme {
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

body {
  margin: 0;
  background-color: var(--primary-color);
}

.navleft{
  display: flex;
  justify-content: center;
  align-items: center;
}
.navleft h1{
  margin-left: 0.6rem;
}
.links {
  display: flex;
  align-items: center;
  text-align: center;
}

.links img {
  margin: 0 3rem 0 2rem;
  width: 30px;
  cursor: pointer;
}

nav {
  display: flex;
  justify-content: space-between;
  text-align: center;
  padding: 1.2rem;

  img{
    width: 36px;
  }

  h1 {
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

footer {
  display: flex;
  justify-content: space-between;
  text-align: center;
  align-items: center;
  height: 4rem;
  width: 100%;
  bottom: 0;
  top: auto;
}
.footername{
  margin-left: 1.6rem;
}
.socials img{
  width: 36px;
  margin-right: 1.6rem;
}

@media only screen and (max-width: 600px) {
  nav {
    justify-content: flex-end;
    right: 0;

    h1 {
      display: none;
    }
  }
  .links img {
    margin: 0 0 0 5rem;
  }
  .socials img{
    width: 14px;
    margin-right: 0.6rem;
  }
  .footername{
    margin-left: 0.6rem;
    font-size: 12px;
  }
  .copyright{
    font-size: 12px;
  }
}
</style>
