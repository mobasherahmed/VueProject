<template>
  <div class="hello">
    <div class="overlay">
      <div class="container">
        <div class="row">
          <div class="txt col-md-10 text-white right">
            <h1>
              Welcome to My Vue js App
              <br />to fetch the data from API:
              <a href="https://server.offmade.io/code-challenge" target="_blank" rel="noopener noreferrer">
              https://server.offmade.io/code-challenge</a>
            </h1>
            <p class="col-md-12">
              You Can Go to <a href="#"><router-link to="/task"> Task Page </router-link></a>to check That Your API Data Stored in its recommended Place.
            </p>
            <form class="form-inline">
              <button class="btn btn-outline-success m-2 my-sm-0" type="submit">Get Started</button>
            </form>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  background: linear-gradient(0deg, rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.4)),
    url(../assets/home-banner.jpg) no-repeat scroll center;
  background-size: cover;
  height: auto;
}
.overlay {
  background-color: rgba(0, 0, 0, 0.6);
  height: auto;
}
.right {
  padding: 30px;
  margin: 100px auto;
}
.form-inline button {
  margin: 0 auto !important;
}
.boxes {
  position: relative;
  top: 0rem;
}
.boxes .boxes-item {
  text-align: center;
  background: linear-gradient(90deg, #e94086 0%, #e5925a 100%);
  margin: 10px 0;
  width: 80% !important;
  padding: 10px;
  color: white;
}
.boxes .boxes-item:nth-child(2) {
  background: linear-gradient(90deg, #7349cc 0%, #e163e4 100%);
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
  text-decoration: none;
  display: inline;
}
a:hover{
   text-decoration: none;
}
.task{
  color:#42b983
}

</style>
