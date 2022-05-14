<template>
  <div class="homeinfo">
    <h1 class="iam">Hi, i'm <span class="stef">Stef</span></h1>
    <h1>I'M A C# AND WEB DEVELOPER</h1>
    <h4>I'm a student at Hogeschool PXL. I make websites and C# applications</h4>
  </div>
</template>

<style>

.homeinfo {
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: left;
  margin-left: 10rem;
  width: 60%;
  min-height: 81vh;
}
.iam{
  font-size: 46px;
}
h1{
  margin: 0.2rem;
}
h2{
  margin: 0.2rem;
}
h4{
  margin: 0.2rem;
}
.stef {
  color: #42b983;
}

@media only screen and (max-width: 600px){
  .homeinfo{
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
