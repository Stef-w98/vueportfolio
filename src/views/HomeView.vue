<template>
  <div class="homeinfo">
    <section>
      <h1 class="iam">Hi, i'm</h1>
      <div class="content">
        <h2>Stef</h2>
        <h2>Stef</h2>
      </div>
    </section>
    <h1>I'M A C# AND WEB DEVELOPER</h1>
    <h4>I'm a student at Hogeschool PXL. I make websites and C# applications</h4>
  </div>
</template>

<style>

@import url("https://fonts.googleapis.com/css?family=Poppins:100,200,300,400,500,600,700,800,900");

.content {
  position: relative;
}

.content h2 {
  color: #fff;
  font-size: 8em;
  position: absolute;
  transform: translate(150px, -130px);
}

.content h2:nth-child(1) {
  color: transparent;
  -webkit-text-stroke: 2px #42b983;
}

.content h2:nth-child(2) {
  color: #42b983;
  animation: animate 4s ease-in-out infinite;
}

@keyframes animate {
  0%,
  100% {
    clip-path: polygon(
        0% 45%,
        16% 44%,
        33% 50%,
        54% 60%,
        70% 61%,
        84% 59%,
        100% 52%,
        100% 100%,
        0% 100%
    );
  }

  50% {
    clip-path: polygon(
        0% 60%,
        15% 65%,
        34% 66%,
        51% 62%,
        67% 50%,
        84% 45%,
        100% 46%,
        100% 100%,
        0% 100%
    );
  }
}

.homeinfo {
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: left;
  margin-left: 10rem;
  width: 60%;
  min-height: 81vh;
}

.iam {
  font-size: 46px;
}

h1 {
  margin: 0.2rem;
}

h2 {
  margin: 0.2rem;
}

h4 {
  margin: 0.2rem;
}

@media only screen and (max-width: 600px) {
  .homeinfo {
    margin-top: 4rem;
    margin-left: 1rem;
  }
}
</style>
<script>
// @ is an alias to /src


export default {
  name: 'HomeView',
  components: {}
}
</script>
