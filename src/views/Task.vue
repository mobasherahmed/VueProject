<template>

  <div class="task-content">
    <div class="container">
      <TaskComp />
    </div>
  </div>

</template>

<script>
// @ is an alias to /src
import TaskComp from "@/components/TaskComp.vue";

export default {
  name: "task",
  components: {
    TaskComp
  }
};
</script>

<style  scoped>
.welcome {
  margin-top: 20px;
}
.task-content{
  height: 100vh;
  background-image: linear-gradient( to left bottom, #051937, #00243e, #002d3b, #003530, #0b3b22 );
}
</style>
