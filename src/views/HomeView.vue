<template>
  <div class="home">
    <h1>Sunethia Lawrence</h1>
    <h2>Aspiring Web Developer</h2>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "HomeView",
 
};
</script>
<style scoped>
.home {
  width: 100vw;
  height: 100vh;
  background-color: #333;
  border: 1px solid black;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
h1 {
  color: white;
  font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS", sans-serif;
  font-size: 3rem;
}
h2 {
  color: white;
}
</style>
