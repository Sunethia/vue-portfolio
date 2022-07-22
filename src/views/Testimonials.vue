<template>
  <div class="testimonials">
    <h1>Testimonials</h1>

    <div class="person" v-for="t of testimonials" :key="t">
      <div class="container">
        <div class="container-inner">
          <img class="circle" :src="t.img" />
        </div>
      </div>
      <div class="divider"></div>
      <div class="name">{{ t.name }}</div>
      <div class="title">" {{ t.text }}"</div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      testimonials: [
        {
          img: "https://i.postimg.cc/QtS1Lh6g/cammy.jpg",
          name: "Cameron Tamboer",
          text: " Sunethia is a very hardworking person, who gives and does her best in all aspects.She also has a very patient and bubbly personality.",
        },
        {
          img: "https://i.postimg.cc/X7rFhM9F/chanique.jpg",
          name: "Chanique Mansoor",
          text: "Sunethia is a very outspoken individual who strives in all aspects and loves taking on challenges. Wishing her all the best  with her future as a developer.",
        },
        {
          img: "https://i.postimg.cc/d1J59TKB/jason.jpg",
          name: "Jason Wandrag",
          text: "I learn something new about Sunethia every day. When she is confident about the answer, she loves participating in class. I'm always happy to see her determined to do well in class. She has learned a lot of new concepts through the duration of the course. Her projects are always improving. If she practices her problem solving more, she will code even more confidently. I enjoy seeing the creative projects she makes, and I hope she practices her coding more! I think Sunethia is a great intern, so she will improve these skills quickly through hard work and studying.",
        },
        {
          img: "https://i.postimg.cc/B6KZC5j1/Muneeb-min.jpg",
          name: "Muneeb Davids",
          text: "Sunethia is a hard working individual who loves what she does and strives in every and every aspect of it.",
        },
        {
          img: "https://i.postimg.cc/c4RQ1w4h/Yasseen.jpg",
          name: "Yaaseen Davids",
          text: " Sunethia is a person that is driven by success and she always puts in the hardwork.",
        },
        {
          img: "https://i.postimg.cc/Pfc6vWHk/zach.jpg",
          name: "Zachary Williams",
          text: " Sunethia Lawrence is a very competent individual, she strives higher than what she is capable of doing.Her passion for her work preference is outstanding and she is a headstrong and smart working person.",
        },
      ],
    };
  },
};
</script>
<style scoped>
.testimonials {
  width: 100vw;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
  background-color: #333;
  flex-wrap: wrap;
}
h1 {
  background-color: #333;
  font-family: "Rampart One";
  font-size: 5rem;
  padding-top: 3rem;
  color: white;
  padding-right: 10rem;
}
/* body {
  align-items: center;
  background-color: #f2f2f2;
  display: flex;
  font-family: "Merriweather", serif;
  flex-wrap: wrap;
  justify-content: center;
  height: 100vh;
  margin: 0;
} */
.person {
  align-items: center;
  display: flex;
  flex-direction: column;
  display: flex;

  /* width: 280px; */
}
.container {
  border-radius: 50%;
  height: 312px;
  -webkit-tap-highlight-color: transparent;
  transform: scale(0.48);
  transition: transform 250ms cubic-bezier(0.4, 0, 0.2, 1);
  width: 400px;
}
.container:after {
  background-color: #f2f2f2;
  content: "";
  height: 10px;
  position: absolute;
  top: 390px;
  width: 100%;
}
.container:hover {
  transform: scale(0.54);
}
.container-inner {
  clip-path: path(
    "M 390,400 C 390,504.9341 304.9341,590 200,590 95.065898,590 10,504.9341 10,400 V 10 H 200 390 Z"
  );
  position: relative;
  transform-origin: 50%;
  top: -200px;
}
.circle {
  background-color: cornflowerblue;
  border-radius: 50%;
  cursor: pointer;
  height: 380px;
  left: 10px;
  pointer-events: none;
  position: absolute;
  top: 210px;
  width: 380px;
}
.img {
  pointer-events: none;
  position: relative;
  transform: translateY(20px) scale(1.15);
  transform-origin: 50% bottom;
  transition: transform 300ms cubic-bezier(0.4, 0, 0.2, 1);
}
.container:hover .img {
  transform: translateY(0) scale(1.2);
}
.img1 {
  left: 22px;
  top: 164px;
  width: 340px;
}
.img2 {
  left: -46px;
  top: 174px;
  width: 444px;
}
.img3 {
  left: -16px;
  top: 144px;
  width: 466px;
}
.divider {
  background-color: cornflowerblue;
  height: 1px;
  width: 160px;
}
.name {
  color: cornflowerblue;
  font-size: 36px;
  font-weight: 600;
  margin-top: 16px;
  text-align: center;
}
.title {
  color: cornflowerblue;
  font-family: arial;
  font-size: 14px;
  font-style: italic;
  margin-top: 4px;
  margin-inline: 20%;
}

@media screen {
  nav {
    display: none;
  }
}
</style>
