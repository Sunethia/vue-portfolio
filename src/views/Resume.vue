<template>
  <div class="container">
    <div class="resume">
      <div class="intro">
        <h1>Sunethia Lawrence</h1>
        <p>Aspiring Full Stack Developer</p>
      </div>
      <div class="left">
        <div class="lefttop">
          <img src="../assets/sunethia.jpg" alt="" />
        </div>
        <div class="leftbottom">
          <h4 class="personal">PERSONAL INFO</h4>
          <br />
          <p class="b">Birth: 23.05.2000</p>
          <p class="b">Country:South-Africa</p>
          <p class="b">City: Cape Town</p>
        </div>
        <!-- <h4 class="contact">CONTACT</h4>
        <div class="conitem">
          <p>Phone :021 952 6731</p>
          <p>Moblie :084 582 8653</p>
          <p style="letter-spacing: 0.2px">Email: lawrencesunethia@gmail.com</p> -->
        <!-- </div> -->
        <h4 class="ed">EDUCATION:</h4>
        <div class="institute">
          <p>
            >High School : D.F Malan High School<br />
            <span style="font-weight: 20; font-size: 9px; letter-spacing: 1px">
              Year Matriculated: 2017 </span
            ><br />2018-2020 Icollege - IT (Technical Support)<br />
            I-Can Genesis Centre- (It Web Specialist/Engineer)
          </p>
          <!-- <div class="peritem">
            <br />
            <p>Birth: 23.05.2000</p>
            <p>Country:South-Africa</p>
            <p>City: Cape Town</p>
          </div> -->
          <!-- <h4 class="contact">CONTACT</h4>
          <div class="conitem">
            <p>Phone :021 952 6731</p>
            <p>Moblie :084 582 8653</p>
            <p style="letter-spacing: 0.2px">
              Email: lawrencesunethia@gmail.com
            </p>
          </div> -->
          <h4 class="ed">EDUCATION</h4>
          <div class="institute">
            <p>
              >High School : D.F Malan High School<br />
              <span
                style="font-weight: 20; font-size: 9px; letter-spacing: 1px"
              >
                Year Matriculated: 2017 </span
              ><br />2018-2020 Icollege - IT (Technical Support)<br />
              I-Can Genesis Centre- (It Web Specialist/Engineer)
              <br />
              <span
                style="font-weight: 20; font-size: 9px; letter-spacing: 1px"
              >
              </span
              ><br />
            </p>
          </div>
        </div>
      </div>
      <div class="ability">
        <div class="circle1">
          <div class="tri1"></div>
          <div class="littlecircle">
            <div class="Design">Ambitious<br />Fearless</div>
          </div>
        </div>
        <div class="circle2">
          <div class="tri2"></div>
          <div class="littlecircle2">
            <div class="markting">Optimistic<br />Reliable</div>
          </div>
        </div>
        <div class="circle3">
          <div class="tri3"></div>
          <div class="littlecircle3">
            <div class="Front-end">Joyful<br />Honest</div>
          </div>
        </div>
      </div>
      <div class="right">
        <div class="profile">
          <h4>PROFILE</h4>
          <hr
            color="#375460"
            size="2px;"
            style="margin-top: 3px; margin-left: 26px; margin-right: 26px"
          />
          <p>
            Hi, I am Sunethia, an aspiring Web developer. I have done a few
            courses in the IT field.In 2018 I did an IT technical support course
            which helped me improve my time management skills.I also did a web
            development course, which taught me the basics of coding. I would
            describe myself as a diligent, hardworking person, with a optimistic
            view on life. I have a bubbly personality and I am always eager to
            learn.Below is five of my greatest attributes.
          </p>
        </div>

        <div class="experience">
          <h4>WORK EXPERIENCE</h4>
          <hr
            color="#375460"
            size="2px;"
            style="margin-top: 3px; margin-left: 26px; margin-right: 26px"
          />
          <div class="tag1">
            2022
            <div class="tagtri1"></div>
          </div>
          <div class="tag2">
            2021
            <div class="tagtri2"></div>
          </div>
          <div class="tag3">
            2020
            <div class="tagtri3"></div>
          </div>

          <div class="verline">
            <div class="spot"></div>
            <div class="spot2"></div>
            <div class="spot3"></div>
            <!-- <div class="spot4"></div> -->
          </div>
          <div class="exitem">
            <div class="it" v-for="w of work" :key="w.name">
              <h4>{{ w.name }}</h4>
              <p>{{ w.title }}</p>
              <h4>Duration: {{ w.duration }}</h4>
              <p>Reference : {{ w.reference.name }}</p>
              <h4>Contact: {{ w.reference.number }}</h4>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      work: [
        {
          name: "Accordion Street Primary School",
          title: "Teachers Assistant",
          duration: "6 months",
          reference: {
            name: " D.Wallenstein",
            number: "073 269 4245",
          },
        },
        {
          name: "Greenchild Project",
          title: "Web Specialist",
          duration: "6 months",
          reference: {
            name: "Edwin Petersen",
            number: "073 599 0312",
          },
        },
        {
          name: "S.A.P.S Parow",
          title: "Telephone operator",
          duration: "6 months",
          reference: {
            name: "Captain K.Williams",
            number: "021 953 8100",
          },
        },
      ],
    };
  },
};
</script>
<style scoped>
h1 {
  font-family: Rampart One;
  color: black;
}
p {
  color: black;
}
p.b {
  padding-right: 3rem;
}

* {
  position: relative;
}

html,
body {
  /* height: 1350px; */
  margin: 0px;
  padding: 0px;
  overflow-x: hidden;
}
.intro {
  box-shadow: 5px 5px 5px 5px black;
  width: 570px;
  border-radius: 10px;
}
.container {
  width: 100vh;
}
.resume {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 20px;
}
.left {
  display: flex;
  justify-content: center;
  align-items: center;
  box-shadow: 5px 5px 5px 5px black;
  border-radius: 10px;
  width: 570px;
  margin-top: 10px;
}
.right {
  display: flex;
  flex-direction: column;
  box-sizing: border-box;
  box-shadow: 5px 5px 5px 5px black;
  margin-bottom: 50px;
  border-radius: 10px;
}

.lefttop img {
  object-fit: cover;
  height: 522px;
  width: 300px;
  margin-bottom: 23rem;
  border-radius: 5rem;
  margin-left: 3rem;
  /* border-radius: 50%; */

  transform: translate(-50px, 60px);
}
.leftbottom {
  width: 306px;
  height: 758px;
  background-color: white;
  font-family: HelveticaNeue-Condensed;
  color: black;
  padding-top: 10rem;
  text-align: right;
  border-radius: 10px;
}

.leftbottom h3 {
  letter-spacing: 3px;
  font-size: 30px;
  margin-bottom: 5px;
  margin-top: 0px;
  padding-top: 20px;
}

.leftbottom h4 {
  letter-spacing: 7px;
  font-weight: 50;
}

.personal {
  border-bottom: solid 2px;
  padding-bottom: 12px;
  width: 240px;
  top: 110px;
  position: absolute;

  text-align: left;
}
.contact {
  border-bottom: solid 2px;
  padding-bottom: 12px;
  width: 240px;
  top: 300px;
  position: absolute;
  left: 38px;
  text-align: left;
}
.peritem {
  font-weight: 100;
  padding-bottom: 5px;
  width: 240px;
  top: 160px;
  position: absolute;
  left: 38px;
  text-align: left;
}

.peritem p {
  border-bottom: solid 1px;
  padding-bottom: 2px;
  letter-spacing: 1px;
  margin-left: 2rem;
}

.conitem {
  font-weight: 100;
  padding-bottom: 5px;
  width: 240px;
  top: 350px;
  position: absolute;
  left: 38px;
  text-align: left;
}
.conitem p {
  border-bottom: solid 1px;
  padding-bottom: 2px;
  letter-spacing: 0px;
}

.ed {
  border-bottom: solid 2px;
  padding-bottom: 12px;
  width: 240px;
  top: 515px;
  position: absolute;

  left: 18.5rem;
  text-align: left;
}

.institute {
  font-weight: 100;
  width: 240px;
  top: 575px;
  position: absolute;
  left: 38px;
  text-align: left;
  font-size: 12px;
  letter-spacing: 1px;
  /* border-bottom: solid 1px; */
}
.institute p {
  line-height: 20px;
  padding-bottom: 0px;
  margin-bottom: 3px;
  text-align: right;
  left: 13rem;
}

.leftbottom span {
  font-weight: 60;
  letter-spacing: 3px;
}

.leftbottom,
.lefttop {
  box-sizing: border-box;
}

.icons {
  width: 240px;
  height: 60px;
  position: absolute;
  left: 27px;
  top: 800px;
}

.fb {
  width: 50px;
  height: 50px;
  position: absolute;
  left: 10px;
  top: 5px;
  line-height: 50px;
  background-image: url(https://static.wixstatic.com/media/95924b_fad19adafcb047e98b534b2ce396808a~mv2.png);
  background-size: cover;
}

.behance {
  width: 50px;
  height: 50px;
  position: absolute;
  left: 95px;
  top: 5px;
  line-height: 50px;
  background-image: url(https://static.wixstatic.com/media/95924b_f3b5d4603227407fbf237227d0201031~mv2.png);
  background-size: cover;
}

.medium {
  width: 50px;
  height: 50px;
  position: absolute;
  left: 180px;
  top: 5px;
  line-height: 50px;
  background-image: url(https://static.wixstatic.com/media/95924b_01ab2c5f473d4f7d98cd651e2220ce44~mv2.png);
  background-size: cover;
}

.right {
  width: 556px;
  background-color: white;
}

.right h4 {
  color: black;
  width: 240px;
  left: 28px;
  text-align: left;
  margin-bottom: -1px;
  letter-spacing: 7px;
}
.profile p {
  text-align: justify;
  text-justify: distribute;
  width: 495px;
  left: 28px;
  letter-spacing: 0.2px;
  color: black;
}
.ability {
  display: flex;
  justify-content: center;
  align-items: center;
}

.circle1,
.circle2,
.circle3 {
  display: inline-block;
  width: 120px;
  height: 120px;
  margin-left: 33.15px;
  border-radius: 100%;
  background-color: black;
  overflow: hidden;
}

.tri1 {
  left: 46px;
  width: 0px;
  height: 0px;
  border-top: 60px solid transparent;
  border-bottom: 60px solid transparent;
  border-right: 90px solid lightsteelblue;
  transform-origin: 0px 60px;
  transform: rotate(-125deg);
  margin-right: auto;
  margin-left: auto;
}

.tri2 {
  left: 70px;
  bottom: 28px;
  width: 0px;
  height: 0px;
  border-top: 90px solid transparent;
  border-bottom: 90px solid transparent;
  border-right: 90px solid lightsteelblue;
  transform-origin: -12px 95px;
  transform: rotate(-125deg);
  margin-right: auto;
  margin-left: auto;
}

.tri3 {
  left: 46px;
  bottom: 120px;
  width: 0px;
  height: 0px;
  border-top: 180px solid transparent;
  border-bottom: 180px solid transparent;
  border-right: 90px solid lightsteelblue;
  transform-origin: 0px 180px;
  transform: rotate(-125deg);
  margin-right: auto;
  margin-left: auto;
}

.littlecircle {
  width: 100px;
  height: 100px;
  margin-left: auto;
  margin-right: auto;
  top: -110px;
  border-radius: 100%;
  background-color: #fffffc;
}

.Design {
  width: 100px;
  height: 100px;
  box-sizing: border-box;
  position: absolute;
  text-align: center;
  font-size: 15px;
  line-height: 25px;
  padding-top: 22.5px;
  color: #6495aa;
}

.littlecircle2 {
  width: 100px;
  height: 100px;
  margin-left: auto;
  margin-right: auto;
  top: -170px;
  border-radius: 100%;
  background-color: #fffffc;
}

.markting {
  width: 100px;
  height: 100px;
  box-sizing: border-box;
  position: absolute;
  text-align: center;
  font-size: 15px;
  line-height: 95px;
  color: #6495aa;
}

.littlecircle3 {
  width: 100px;
  height: 100px;
  right: 10px;
  top: 10px;
  border-radius: 100%;
  background-color: #fffffc;
  position: absolute;
}

.Front-end {
  width: 100px;
  height: 100px;
  box-sizing: border-box;
  position: absolute;
  text-align: center;
  font-size: 15px;
  line-height: 25px;
  padding-top: 22.5px;
  color: #6495aa;
}

.experience {
  height: 400px;
  box-sizing: border-box;
  margin-inline: 8%;
}
.experience h4 {
  color: black;
  width: 300px;
  left: 28px;
  text-align: left;
  margin-bottom: -1px;
  letter-spacing: 7px;
}
.tag1 {
  background-color: #6495aa;
  width: 100px;
  height: 34px;
  left: 28px;
  top: 64px;
  position: absolute;
  font-weight: 80;
  text-align: left;
  font-size: 18px;
  line-height: 34px;
  color: white;
  letter-spacing: 4px;
}

.tagtri1 {
  width: 0px;
  height: 1px;
  border-top: 16.5px solid transparent;
  border-bottom: 16.5px solid transparent;
  border-left: solid 20px #6495aa;
  position: absolute;
  left: 100px;
  top: 0px;
}

.tag2 {
  background-color: #6495aa;
  width: 100px;
  height: 34px;
  left: 28px;
  top: 215px;
  position: absolute;
  text-align: left;
  font-size: 18px;
  font-weight: 80;
  line-height: 34px;
  color: black;
  letter-spacing: 4px;
}

.tagtri2 {
  width: 0px;
  height: 1px;
  border-top: 16.5px solid transparent;
  border-bottom: 16.5px solid transparent;
  border-left: solid 20px #6495aa;
  position: absolute;
  left: 100px;
  top: 0px;
}

.tag3 {
  background-color: #6495aa;
  width: 100px;
  height: 34px;
  left: 28px;
  top: 319px;
  position: absolute;
  text-align: left;
  font-size: 18px;
  font-weight: 80;
  line-height: 34px;
  color: black;
  letter-spacing: 4px;
}

.tagtri3 {
  width: 0px;
  height: 1px;
  border-top: 16.5px solid transparent;
  border-bottom: 16.5px solid transparent;
  border-left: solid 20px #6495aa;
  position: absolute;
  left: 100px;
  top: 0px;
}

.tag4 {
  background-color: #6495aa;
  width: 100px;
  height: 34px;
  left: 28px;
  top: 470px;
  position: absolute;
  text-align: left;
  font-size: 18px;
  font-weight: 80;
  line-height: 34px;
  color: black;
  letter-spacing: 4px;
}

.tagtri4 {
  width: 0px;
  height: 1px;
  border-top: 16.5px solid transparent;
  border-bottom: 16.5px solid transparent;
  border-left: solid 20px #6495aa;
  position: absolute;
  left: 100px;
  top: 0px;
}

.verline {
  width: 1px;
  height: 300px;
  background-color: #375460;
  position: absolute;
  left: 165px;
  top: 82px;
}

.spot {
  width: 16px;
  height: 16px;
  right: 7px;
  border-radius: 100%;
  background-color: #375460;
  top: -10px;
}

.spot2 {
  width: 16px;
  height: 16px;
  right: 7px;
  border-radius: 100%;
  background-color: #375460;
  top: 126px;
}

.spot3 {
  width: 16px;
  height: 16px;
  right: 7px;
  border-radius: 100%;
  background-color: #375460;
  top: 215px;
}

.spot4 {
  width: 16px;
  height: 16px;
  right: 7px;
  border-radius: 100%;
  background-color: #375460;
  top: 350px;
}

.exitem {
  width: 350px;
  height: 500px;
  left: 180px;
  top: 70px;
  position: absolute;
  box-sizing: border-box;
}
.exitem h4 {
  font-size: 13px;
  width: 350px;
  left: 0px;
  letter-spacing: 3px;
  margin-top: 0px;
}
.exitem p {
  margin-top: 0px;
  margin-bottom: 5px;
  color: white;
}

.software,
.language {
  display: inline-block;
  box-sizing: border-box;
}

.software {
  width: 277px;
  height: 255px;
  margin-top: 5px;
}

.software h4 {
  margin-top: 7px;
  margin-bottom: 0px;
}

.psbar {
  height: 50px;
  padding-top: 0px;
  margin-left: 26px;
  font-size: 6px;
  letter-spacing: 2px;
  color: rgba(0, 0, 0, 0.55);
}

.barchart1 {
  margin-top: 3px;
  height: 20px;
  width: 240px;
  background-color: #dbdbd9;
}

.value1 {
  height: 20px;
  width: 200px;
  margin-right: auto;
  background-color: #6495aa;
}

.aibar {
  height: 50px;
  padding-top: 0px;
  margin-left: 26px;
  font-size: 6px;
  letter-spacing: 2px;
  color: rgba(0, 0, 0, 0.55);
}

.barchart2 {
  margin-top: 3px;
  height: 20px;
  width: 240px;
  background-color: #dbdbd9;
}

.value2 {
  height: 20px;
  width: 220px;
  margin-right: auto;
  background-color: #6495aa;
}

.idbar {
  height: 50px;
  padding-top: 0px;
  margin-left: 26px;
  font-size: 6px;
  letter-spacing: 2px;
  color: rgba(0, 0, 0, 0.55);
}

.barchart3 {
  margin-top: 3px;
  height: 20px;
  width: 240px;
  background-color: #dbdbd9;
}

.value3 {
  height: 20px;
  width: 180px;
  margin-right: auto;
  background-color: #6495aa;
}

.lrbar {
  height: 50px;
  padding-top: 0px;
  margin-left: 26px;
  font-size: 6px;
  letter-spacing: 2px;
  color: rgba(0, 0, 0, 0.55);
}

.barchart4 {
  margin-top: 3px;
  height: 20px;
  width: 240px;
  background-color: #dbdbd9;
}

.value4 {
  height: 20px;
  width: 200px;
  margin-right: auto;
  background-color: #6495aa;
}

.language {
  width: 277px;
  height: 255px;
  margin-top: 5px;
}

.language h4 {
  margin-top: 7px;
  margin-bottom: 0px;
}

.language p {
  font-size: 13px;
  color: rgba(0, 0, 0, 0.55);
  margin-top: 0px;
  border-bottom: solid 0.5px;
  margin-left: 18px;
  margin-bottom: 0px;
  margin-right: 26px;
  letter-spacing: 2px;
}

.mabar {
  width: 95px;
  height: 130px;
  margin-top: 0px;
  background-color: rgba(100, 149, 179, 0.75);
  margin-left: 156px;
}

.english {
  width: 259px;
  position: absolute;
  top: 50px;
  margin-left: 18px;
}

.english p {
  margin-left: 0px;
  border-bottom: solid 0.5px;
  width: 173px;
}

.enbar {
  width: 95px;
  height: 80px;
  margin-top: 0px;
  background-color: rgba(55, 84, 96, 0.75);
  margin-left: 78px;
}

.jpn {
  width: 259px;
  position: absolute;
  top: 99px;
  margin-left: 18px;
}

.jpn p {
  margin-left: 0px;
  border-bottom: solid 0.5px;
  width: 115px;
}

.jpbar {
  width: 95px;
  height: 31px;
  margin-top: 0px;
  background-color: rgba(164, 185, 193, 0.45);
  margin-left: 20px;
}

.lancube {
  margin-top: 26px;
  font-size: 2px;
  color: rgba(0, 0, 0, 0.55);
  width: 259px;
  left: 18px;
}

.cube1 {
  width: 15px;
  height: 15px;
  display: inline-block;
  background-color: rgba(100, 149, 179, 0.75);
  top: -2px;
}

.cube2 {
  width: 15px;
  height: 15px;
  display: inline-block;
  background-color: rgba(55, 84, 96, 0.75);
  left: 20px;
  top: -2px;
}

.cube3 {
  width: 15px;
  height: 15px;
  display: inline-block;
  background-color: rgba(164, 185, 193, 0.45);
  left: 68px;
  top: -2px;
}

.it {
  width: 280px;
  margin: 2px;
}
/* media queries */

@media (min-width: 700px) and (max-width: 850px) {
  .profile p {
    font-size: 16px;
  }
  .ability {
    display: none;
  }
  h4 {
    display: flex;
  }
}
@media (min-width: 300px) and (max-width: 850px) {
  .profile p {
    font-size: 16px;
  }
  .ability {
    display: none;
  }
}
</style>
