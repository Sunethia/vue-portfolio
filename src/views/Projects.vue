<template>
  <div class="container">
    <div class="projects">
      <h1 class="title">Projects</h1>
      <div class="card" v-for="p of projects" :key="p">
        <img class="card-img-top" :src="p.img" alt="Card image cap" />
        <div class="card-body">
          <h5 class="card-title">{{ p.title }}</h5>
          <p class="card-text">
            {{ p.text }}
          </p>
          <a :href="p.git" class="btn btn-primary">Github</a>
          <a :href="p.live" class="btn btn-primary">Live</a>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      projects: [
        {
          img: "https://i.postimg.cc/zGyk268Q/bmi.jpg",
          title: "BMI calculator",
          text: "BMI calculator, calculates your body mass index and tells you if you are the right weight for your age/height",
          git: "https://github.com/Sunethia/bmi_calculator",
          live: "https://vocal-pie-c313a9.netlify.app",
        },
        {
          img: "https://i.postimg.cc/44rLkXFg/cal.jpg",
          title: "Calculator",
          text: "This is a functional calculator, which can be used on a phone or laptop",
          git: "https://github.com/Sunethia/Calculator",
          live: "https://statuesque-beignet-53784f.netlify.app",
        },
        {
          img: "https://i.postimg.cc/662Kf5vJ/code.jpg",
          title: "My First Portfolio",
          text: "This is my first portfolio created with only HTML and CSS.",
          git: "https://github.com/Sunethia/My-Portfolio",
          live: "https://resilient-gelato-697c23.netlify.app",
        },
        {
          img: "https://i.postimg.cc/7Ytg89LT/houzez.jpg",
          title: "Properties",
          text: "This website allows you to look at apartments or houses,which is either for rent or sale",
          git: "https://github.com/Sunethia/houzez.git",
          live: "https://harmonious-chimera-1400b0.netlify.app",
        },
        {
          img: "https://i.postimg.cc/8c6VptSP/todo.jpg",
          title: "To-do List",
          text: "This is a to-do list, which allows you to add and delete items",
          git: "https://github.com/Sunethia/to-do-list",
          live: "https://enchanting-gaufre-33a4a3.netlify.app",
        },
        {
          img: "https://i.postimg.cc/c43Ds6vm/restaurant.jpg",
          title: "Restaurantly",
          text: "This website is a website of restaurant where you are able to book a table at the restaurant.",
          git: "https://github.com/Sunethia/Restaurant",
          live: "https://velvety-hummingbird-230f0d.netlify.app",
        },
      ],
    };
  },
};
</script>
<style>
.projects {
  background-color: #333;
  height: 100vh;
  display: flex;
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
.card {
  width: 16rem;
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  align-items: center;
  background-color: #333;
}
.container {
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
h5.card-title {
  color: white;
}
p.card-text {
  color: white;
}
</style>
