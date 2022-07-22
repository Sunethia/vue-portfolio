<template>
  <div class="about">
    <div class="container">
      <div class="row">
        <div class="col">
          <img src="../assets/avatar.jpg" alt="avatar" />
        </div>
        <div class="col">
          <h1>Ohh, Hi There!</h1>
          <h2>
            My name is Sunethia Haimly Lawrence.I am an Aspiring web
            developer,<br />
            located in South Africa, Cape town.*** I regard myself as a<br />
            loving,caring and loyal person. I surround myself with people who<br />
            inspires me to become a better person.Being myself and humble
            <br />at all times, I believe has brought me this far.<br />I adapt
            to situations and regard myself as a diligent and <br />hardworking
            individual. My eagerness is one of my greatest attributes.
          </h2>
        </div>
      </div>
      <div class="scroll-downs">
        <div class="mousey">
          <div class="scroller"></div>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
.about {
  height: 100vh;
  background-color: #333;
}

h1 {
  font-family: Rampart One;
  color: white;
  display: flex;
  justify-content: center;
  padding-top: 8rem;
  margin-bottom: 2rem;
}
h2 {
  color: white;
  font-size: 1rem;
  display: flex;
  align-items: center;
  justify-content: center;
  padding-bottom: 5rem;
}
img {
  border: 2px solid cornflowerblue;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 10rem;
  margin-left: 9rem;
  box-shadow: 5px 5px 5px 5px blue;
}
/* animation */
body,
html {
  background-color: cornflowerblue;
  width: 100%;
  min-height: 100%;
  padding: 0;
  margin: 0;
}
.scroll-downs {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  margin: auto;

  width: 36px;
  height: 55px;
}
.mousey {
  width: 10px;
  padding: 10px 15px;
  height: 50px;
  border: 4px solid cornflowerblue;
  border-radius: 25px;
  opacity: 0.75;
  box-sizing: content-box;
}
.scroller {
  width: 3px;
  height: 10px;
  border-radius: 25%;
  background-color: cornflowerblue;
  animation-name: scroll;
  animation-duration: 2.2s;
  animation-timing-function: cubic-bezier(0.15, 0.41, 0.69, 0.94);
  animation-iteration-count: infinite;
}
@keyframes scroll {
  0% {
    opacity: 0;
  }
  10% {
    transform: translateY(0);
    opacity: 1;
  }
  100% {
    transform: translateY(15px);
    opacity: 0;
  }
}
/* media queries */
@media (min-width: 300px) and (max-width: 1285px) {
  .about h1 {
    font-size: 3rem;
  }
  .about h2 {
    font-size: 1rem;
  }
}
@media (min-width: 300px) and (max-width: 990px) {
  .about h1 {
    font-size: 3rem;
  }
  .about h2 {
    font-size: 1rem;
    margin-inline: 10%;
  }
  .about img {
    margin-bottom: 2px;
    margin-top: 10rem;
    margin-left: 2rem;
    width: 15rem;
  }
  .about h1 {
    font-size: 2rem;
    padding-top: 5rem;
    padding-right: -5px;
  }
}
@media (min-width: 300px) and (max-width: 350px) {
  .about img {
    width: 13rem;
    margin-top: -0.2rem;
    margin-top: 5rem;
  }
  .about h1 {
    font-size: 1rem;
    margin-top: -3.5rem;
  }
  .about h2 {
    font-size: 0.9rem;
  }
  .about mousey {
    margin-top: 22rem;
  }
}
</style>
<script></script>
