<template>
  <div class="task-comp">
    <div class="container">
      <div class="row">
        <div class="content col-md-5">
          <h4>Purchase price</h4>
          <div class="d-flex">
            <input type="text" class="form-control" :value="post.price" />
            <div class="d-flex dollar">
              <h5 class="mx-2">$</h5>
              <button
                class="btn btn-outline-secondary dropdown-toggle"
                type="button"
                data-toggle="dropdown"
                aria-haspopup="true"
                aria-expanded="false"
              ></button>
              <div class="dropdown-menu">
                <a class="dropdown-item" href="#">{{post.currency}}</a>
              </div>
            </div>
          </div>
        </div>

        <div class="content col-md-5">
          <h4>Plot size</h4>
          <div class="d-flex">
            <input type="text" class="form-control" :value="post.plotSize" />
            <h6>
              | m
              <sup>2</sup>
            </h6>
          </div>
        </div>

        <div class="content col-md-5">
          <h4>Years of construction</h4>
          <input type="text" class="form-control" :value="post.yearOfConstruction" />
        </div>

        <div class="content col-md-5">
          <h4>Net rent total (p.a.)</h4>
          <div class="d-flex">
            <input type="text" class="form-control" :value="post.netRentTotal" />
            <h5>| $/p.a.</h5>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
import axios from "axios";
export default {
  name: "TaskComp",
  data() {
    return {
      post: []
    };
  },
  mounted() {
    var self = this;
    axios.get("https://server.offmade.io/code-challenge").then(function(res) {
      self.post = res.data;
      console.log("Data :", self.post);
    });
  }
};
</script>


<style scoped>
.task-comp {
  text-align: center;
  padding: 20px 0;
}
h4 {
  color: white;
}
h5 {
  margin-left: -70px;
  margin-top: 5px;
  color: #ccc;
}

.dollar {
  margin-left: -60px;
}
h6 {
  margin-left: -40px;
  margin-top: 8px;
  color: #ccc;
}
button {
  border: transparent;
}
button:hover {
  border: transparent;
  background-color: seagreen;
}
.dropdown-menu {
  min-width: 5rem;
}
.show {
  left: -30px !important;
}
.content {
  padding: 50px;
  text-align: center;
}
</style>
