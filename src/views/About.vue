<template>
  <div class="about">
    <div class="overlay">
      <div class="container">
        <div class="row">
          <div class="main-title">
            <h1>About Me</h1>
            <p class="col-md-5">
              I'M
              <span class="flag">AHMED HASSAN MOBASHER</span> :
              Self-motivated web developer with a creative eye for design and proficient at crafting projects from beginning to end ,
              Looking to shift away from design to focus more on development ,
              willing to have an opportunity to prove my skills and develop it .
            </p>
            <div class="divider"></div>
            <div class="second-title d-flex">
              <h6>Home</h6>
              <span class="flag">=></span>
              <h6>About</h6>
            </div>
            <div class="divider"></div>
            <div class="links">
              <div class="d-flex">
              <a href="https://www.linkedin.com/in/ahmed-mobasher-10/" target="_blank" rel="noopener noreferrer" class="mx-2">
              <i>LinkedIn</i>
              </a>
              <a href="https://github.com/mobasherahmed" target="_blank" rel="noopener noreferrer" class="mx-2">
              <i>GitHub</i>
              </a>
            </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import "@/assets/fonts/fontawesome.min.css";

export default {
  name: "home"
};
</script>

<style  scoped>
.overlay {
  background-color: rgba(0, 0, 0, 0.6);
  height: auto;
}
.about {
  background: linear-gradient(0deg, rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.4)),
    url(../assets/home-banner.jpg) no-repeat scroll center;
  background-size: cover;
  height: auto;
}
.second-title {
  margin: 10px calc(50% - 50px);
}
.divider {
  background-color: white;
  width: 150px;
  height: 1.5px;
  margin: 10px calc(50% - 80px);
}
.main-title {
  padding: 100px 0;
}
.main-title p {
  margin: 0 auto;
}
.main-title p:hover {
  color: #42b983;
  transition: 2s all ease-in-out;
}
.main-title p:hover .flag {
  color: white;
  transition: 2s all ease-in-out;
}
.flag {
  color: #42b983;
}
.links .d-flex{
  margin:0 calc(41%)
}
</style>
