<template>
  <div class="testimonials">
    <div class="person">
      <div class="container">
        <div class="container-inner">
          <img class="circle" src="../assets/chanique.jpg" />
        </div>
      </div>
      <div class="divider"></div>
      <div class="name">Chanique Mansoor</div>
      <div class="title">
        "Sunethia is a very energetic and bright<br />
        person who lights up the room with her<br />
        personality, she works very hard on succeeding and<br />
        is passionate about the work she does.<br />
        You'll never have a dull moment with her around."
      </div>
    </div>
    <div class="person">
      <div class="container">
        <div class="container-inner">
          <img class="circle" src="../assets/Muneeb-min.jpg" />
        </div>
      </div>
      <div class="divider"></div>
      <div class="name">Muneeb Davids</div>
      <div class="title">
        "Sunethia is a hard working individual who loves what she does<br />
        and strives in every and every aspect of it."
      </div>
    </div>
    <div class="person">
      <div class="container">
        <div class="container-inner">
          <img class="circle" src="../assets/Yasseen.jpg" />
        </div>
      </div>
      <div class="divider"></div>
      <div class="name">Yaaseen Davids</div>
      <div class="title">
        Sunethia is a person that is driven by<br />
        success and she always puts in the hardwork.
      </div>
    </div>
    <div class="person">
      <div class="container">
        <div class="container-inner">
          <img class="circle" src="../assets/cammy.jpg" />
        </div>
      </div>
      <div class="divider"></div>
      <div class="name">Cameron Tamboer</div>
      <div class="title">
        Sunethia is a very hardworking person,<br />
        who gives and does her best in all aspects.<br />
        She also has a very patient and bubbly personality.<br />
      </div>
    </div>
    <div class="person">
      <div class="container">
        <div class="container-inner">
          <img class="circle" src="../assets/Jason.jpg" />
        </div>
      </div>
      <div class="divider"></div>
      <div class="name">Jason Wandrag</div>
      <div class="title">
        "Sunethia is a hard working individual who loves what she does<br />
        and strives in every and every aspect of it."
      </div>
    </div>
    <div class="person">
      <div class="container">
        <div class="container-inner">
          <img class="circle" src="../assets/zach.jpg" />
        </div>
      </div>
      <div class="divider"></div>
      <div class="name">Zachary Williams</div>
      <div class="title">
        Sunethia Lawrence is a very<br />
        competent individual, she strives higher<br />
        than what she is capable of doing.<br />
        Her passion for her work <br />preference is outstanding and she<br />
        is a headstrong and smart working person."
      </div>
    </div>
    
  </div>
</template>
<script>
export default {};
</script>
<style>
.testimonials {
  width: 100vw;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
  background-color: #333;
  flex-wrap: wrap;
}
body {
  align-items: center;
  background-color: #f2f2f2;
  display: flex;
  font-family: "Merriweather", serif;
  flex-wrap: wrap;
  justify-content: center;
  height: 100vh;
  margin: 0;
}
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
}

@media screen {
  nav {
    display: none;
  }
}
</style>
