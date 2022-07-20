<template>
  <div class="container">
    <div class="projects">
      <h1 class="title">Projects</h1>
      <div class="card" style="width: 18rem">
        <img
          class="card-img-top"
          src="../assets/code-back.jpg"
          alt="Card image cap"
        />
        <div class="card-body">
          <h5 class="card-title">My First Portfolio</h5>
          <p class="card-text">
            This is a portfolio that I created using HTML and CSS.
          </p>
          <a
            href="https://github.com/Sunethia/My-Portfolio"
            class="btn btn-primary"
            >Github</a
          >
          <a
            href="https://resilient-gelato-697c23.netlify.app"
            class="btn btn-primary"
            >Live</a
          >
        </div>
      </div>
      <div class="card" style="width: 18rem">
        <img
          class="card-img-top"
          src="../assets/cal.jpg"
          alt="Card image cap"
        />
        <div class="card-body">
          <h5 class="card-title">Calculator</h5>
          <p class="card-text">
            This is a Calculator, that can be used on a phone or laptop.
          </p>
          <a
            href="https://github.com/Sunethia/Calculator"
            class="btn btn-primary"
            >Github</a
          >
          <a
            href="https://statuesque-beignet-53784f.netlify.app"
            class="btn btn-primary"
            >Live</a
          >
        </div>
      </div>
      <div class="card" style="width: 18rem">
        <img
          class="card-img-top"
          src="../assets/bmi.jpg"
          alt="Card image cap"
        />
        <div class="card-body">
          <h5 class="card-title">BMI Calculator</h5>
          <p class="card-text">
            This is a calculator that calculates your body mass index and tells
            you if you overweight or not.
          </p>
          <a
            href="https://github.com/Sunethia/bmi_calculator"
            class="btn btn-primary"
            >Github</a
          >
          <a href="https://vocal-pie-c313a9.netlify.app" class="btn btn-primary"
            >Live</a
          >
        </div>
      </div>
      <div class="card" style="width: 18rem">
        <img
          class="card-img-top"
          src="../assets/todo.jpg"
          alt="Card image cap"
        />
        <div class="card-body">
          <h5 class="card-title">To do list</h5>
          <p class="card-text">
            To do list, where you can add and delete items.
          </p>
          <a
            href="https://github.com/Sunethia/to-do-list"
            class="btn btn-primary"
            >Github</a
          >
          <a
            href="https://enchanting-gaufre-33a4a3.netlify.app"
            class="btn btn-primary"
            >Live</a
          >
        </div>
      </div>
      <div class="card" style="width: 18rem">
        <img
          class="card-img-top"
          src="../assets/houzez.jpg"
          alt="Card image cap"
        />
        <div class="card-body">
          <h5 class="card-title">Property Store</h5>
          <p class="card-text">
            This is a site where you can purchase apartments and houses,prices
            and locations is included.
          </p>
          <a href="https://github.com/Sunethia/houzez" class="btn btn-primary"
            >Github</a
          >
          <a
            href="https://harmonious-chimera-1400b0.netlify.app"
            class="btn btn-primary"
            >Live</a
          >
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style>
div.projects {
  background-color: #333;
  height: 100vh;
}
.title[margin-top: 2rem;] .card {
  border: 1px solid black;
  width: 4rem;
  height: 25rem;
}
.card-img-top {
  width: 13.7rem;
  height: 12rem;
}
div.card {
  width: 16rem;
    display: flex;
    justify-content: space-between;
    flex-direction:column;
    align-items: center;
}
div.container {
  display: flex;
  justify-content: center;
  flex-direction: row;
  align-items: center;
  gap: 3rem;
  background-color: #333;
}
.title {
  background-color: #333;
}
div#app {
  background-color: #333;
}
</style>
