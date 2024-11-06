<template>
  <q-page class="flex flex">
    <!-- <img class="image" src="/3815805.jpg" alt="coding" /> -->

    <div class="box" id="box"></div>
    <div class="divTit">
      <h2 class="title">Front-End Developer<span class="hand">👋🏻</span></h2>

      <h5 class="aaa" style="margin-bottom: 0%">
        Hi, I'm Taha Jamalizade.A passionate Front-end Developer <br />
        based in Qom & Tehran. 📍
      </h5>
      <a target="_blank" href="https://github.com/tahajam8304">
        <img
          style="margin-bottom: 4%"
          class="github"
          src="/public/github-mark.svg"
          alt=""
        />
      </a>
      <div style="display: flex">
        <h6 class="tech" style="margin: 0%">Tech Stack |</h6>
        <img class="html" src="/icons8-html.svg" alt="html" />
        <img
          style="margin-left: 1%"
          class="html"
          src="icons8-css.svg"
          alt="css"
        />
        <img class="html" src="icons8-javascript.svg" alt="javascript" />
        <img
          style="margin-left: 3%"
          class="html"
          src="icons8-vue-js.svg"
          alt="vue"
        />
        <img
          style="margin-left: 3px"
          class="html"
          src="quasar-svgrepo-com.svg"
          alt="quasar"
        />
        <img class="html" id="word" src="wordpress.svg" alt="" />
      </div>
      <br />
    </div>
    <div id="about" style="display: flex; margin-top: 40px; margin-left: 20px">
      <div class="progres">
        <div class="progress" style="margin-top: 70px; display: flex">
          <h5 style="margin-top: 0%; margin-right: 30px; color: #f40057">
            HTML
          </h5>
          <q-linear-progress
            size="25px"
            :value="HTML"
            color="pink-13"
            style="border-radius: 30px"
          >
            <div class="absolute-full flex flex-center">
              <q-badge
                color="white"
                text-color="pink-13"
                :label="progressLabel1"
              />
            </div>
          </q-linear-progress>
        </div>

        <div
          class="progress"
          style="margin-top: 0px; display: flex;"
        >
          <h5 style="margin-top: 0px; margin-right: 30px; color: #f40057">
            CSS
          </h5>
          <q-linear-progress
            size="25px"
            :value="CSS"
            color="pink-13"
            style="border-radius: 30px"
          >
            <div class="absolute-full flex flex-center">
              <q-badge color="white" text-color="pink-13" :label="CSSLabel1" />
            </div>
          </q-linear-progress>
        </div>

        <div class="progress" style="display: flex">
          <h5 style="color: #f40057; margin-top: 0%; margin-right: 45px">JS</h5>
          <q-linear-progress
            size="25px"
            :value="JAVASCRIPT"
            color="pink-13"
            style="border-radius: 30px"
          >
            <div class="absolute-full flex flex-center">
              <q-badge
                color="white"
                text-color="pink-13"
                :label="JAVASCRIPTLabel1"
              />
            </div>
          </q-linear-progress>
        </div>
        <div class="progress" style="display: flex">
          <h5 style="color: #f40057; margin-top: 0%; margin-right: 45px">
            vue
          </h5>
          <q-linear-progress
            size="25px"
            :value="vue"
            color="pink-13"
            style="border-radius: 30px"
          >
            <div class="absolute-full flex flex-center">
              <q-badge color="white" text-color="pink-13" :label="vueLabel1" />
            </div>
          </q-linear-progress>
        </div>
      </div>
      <img
        class="laptop"
        src="/LAPTOP.jpg"
        alt="laptop"
        style="margin-left: 0%"
      />
      <div>
        <h5 class="me">About me</h5>
        <h6
          class="amm"
          style="margin-top: 10px; margin-left: 5%; color: rgb(153, 159, 164)"
        >
          Hey, my name is Taha, and I'm a Frontend Developer. <br />My passion
          is to create and develop a clean UI/UX for my users.
        </h6>
      </div>
    </div>
    <div id="projects" class="project">
      <h5 class="protit">Projects</h5>
      <img class="airsheet" src="/airsheet.png" alt="site" />
      <br />
      <div>
        <a class="link" target="_blank" href="https://airsheet.ir/index"
          ><h5 class="link">Click to See the Site</h5></a
        >
      </div>
    </div>
    <div class="contact">
      <h5 class="mee" id="contact">|| CONTACT ||</h5>
      <div class="mail">
        <img class="phon" src="/phone-call-svgrepo-com (1).svg" alt="phone" />
        <h5 style="margin: 0%; color: white" class="title">Phone:</h5>
        <h6 class="phone">+989059229400</h6>
      </div>
      <div class="mail" style="margin-top: 3%">
        <img class="email" src="/email-1-svgrepo-com.svg" alt="" />
        <h5 style="margin: 0%; color: white" class="title">Mail:</h5>
        <a class="phone">mohammad.taha.jam@gmail.com</a>
      </div>
    </div>
    <div></div>

    <div class="ending"></div>
  </q-page>
</template>

<script>
import { defineComponent, ref, computed } from "vue";

export default defineComponent({
  name: "IndexPage",

  setup() {
    const HTML = ref(0.83);
    const CSS = ref(0.64);
    const JAVASCRIPT = ref(0.49);
    const VUE = ref(0.36);

    const progressLabel1 = computed(() => (HTML.value * 100).toFixed(2) + "%");
    const CSSLabel1 = computed(() => (CSS.value * 100).toFixed(2) + "%");
    const JAVASCRIPTLabel1 = computed(
      () => (JAVASCRIPT.value * 100).toFixed(2) + "%"
    );
    const vueLabel1 = computed(() => (VUE.value * 100).toFixed(2) + "%");

    return {
      HTML,
      progressLabel1,
      CSS,
      CSSLabel1,
      JAVASCRIPT,
      JAVASCRIPTLabel1,
      VUE,
      vueLabel1,
    };
  },
});
</script>

<style lang="scss">
///////////dark////////////
///
.body--dark {
  // body {
  //   background-color: #090909;
  // }

  .box {
    width: 400px;
    height: 300px;
    background: url(/3815805.jpg);
    background-position: center;
    background-size: cover;
    position: relative;
    box-shadow: 10px 10px 42px 0px #f40057;
  }
  .box:after {
    animation-delay: -5s;
    background-color: #5995eb;
    clip-path: polygon(
      0 0,
      calc(100% - (33.3333333333px)) calc(0% + (33.3333333333px)),
      100% 100%,
      calc(0% + (33.3333333333px)) calc(100% - (33.3333333333px))
    );
  }
  .box:before {
    background-color: #f40057;
    clip-path: polygon(
      calc(0% + (33.3333333333px)) calc(0% + (33.3333333333px)),
      100% 0,
      calc(100% - (33.3333333333px)) calc(100% - (33.3333333333px)),
      0 100%
    );
  }
  .project {
    background: linear-gradient(
      135deg,
      rgba(86, 83, 83, 0.501),
      rgba(158, 151, 151, 0.544)
    );
    margin: 30px;
  }

  .link {
    color: white;
  }
  .email:hover {
    background: rgb(32, 32, 32);
  }

  .phon:hover {
    background: rgb(32, 32, 32);
  }
}

body {
  background-image: url(/mount.jpg);
}

// .image {
//   width: 30%;
//   height: 20%;
//   border-radius: 50%;
//   border: black solid 5px;
//   margin-top: 4%;
//   margin-left: 37%;
//   animation-name: wave-anim;
//   animation-iteration-count: infinite;
//   transform-origin: 70% 70% 70%;
//   animation-duration: 10s;
// }
@keyframes wave-anim {
  0% {
    transform: rotate(-2deg);
  }
  10% {
    transform: rotate(4deg);
  }
  20% {
    transform: rotate(-7deg);
  }
  30% {
    transform: rotate(7deg);
  }
  40% {
    transform: rotate(-4deg);
  }
  50% {
    transform: rotate(4deg);
  }
  60% {
    transform: rotate(-3deg);
  }
  100% {
    transform: rotate(3deg);
  }
}

.hand {
  animation-name: wave-animation;
  animation-duration: 2.5s;
  animation-iteration-count: infinite;
  transform-origin: 70% 70%;
  display: inline-block;
}
@keyframes wave-animation {
  0% {
    transform: rotate(0deg);
  }
  10% {
    transform: rotate(14deg);
  }
  20% {
    transform: rotate(-8deg);
  }
  30% {
    transform: rotate(14deg);
  }
  40% {
    transform: rotate(-4deg);
  }
  50% {
    transform: rotate(20deg);
  }
  60% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(0deg);
  }
}
.title {
  font-weight: bold;
}
.divTit {
  margin-left: 30%;
  padding-bottom: 0%;
}

.html {
  width: 40px;
  margin-left: 3%;
  transition: 0.4s;
}
.html:hover {
  width: 40px;
  transform: scale(1.5);
}
/* ////////////////// */
.me {
  font-weight: bold;
  color: #f40057;
  margin-bottom: 0%;
  margin-left: 40px;
  margin-top: 100px;
}

.laptop {
  /* border: solid 2px black; */
  border-radius: 40px;
  padding: 1px;
  width: 300px;
  height: 300px;
}
.progres {
  padding-right: 20px;
}
.project {
  width: 100%;
  height: 450px;
  background: linear-gradient(
    135deg,
    rgba(255, 255, 255, 0.1),
    rgba(255, 255, 255, 0)
  );
  margin: 30px;
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border-radius: 20px;
  border: 1px solid rgba(255, 255, 255, 0.18);
  box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.37);
  display: grid;
  justify-content: center;
  margin-top: 4%;
}
.protit {
  font-weight: bold;
  color: #f40057;
  margin-top: 2px;
  justify-content: center;
  display: flex;
  margin-bottom: 20px;
  margin-top: 20px;
}

.airsheet {
  width: 550px;
  height: fit-content;
  // margin-bottom: 20px;
  padding: px;
  // margin-left: 40px;
  border: rgb(158, 155, 155) solid 3px;
  border-radius: 10px;
  // margin-bottom: 0%;
  transition: 0.5s;
  // margin-top: 2px;
  justify-content: center;
  display: flex;
  filter: grayscale(100%);
  cursor: pointer;
}
.airsheet:hover {
  transform: scale(1.1);
  filter: grayscale(0%);
}

.link {
  color: white;
  text-decoration: none;
  margin-top: 0%;
  font-weight: bold;
  display: flex;
  justify-content: center;
  transition: 0.4s;
}
.link:hover {
  color: #f40057;
}
.por {
  color: black;
  font-weight: bold;
  margin-top: 12%;
  font-size: x-large;
}
.mee {
  font-weight: bold;
  color: #f40057;
  margin-left: 19%;
  margin-top: 6%;
}
.contact {
  width: 100%;
  height: 400px;
  margin-top: 0px;
}

.mail {
  margin-left: 19%;
  font-weight: bold;
}

.phone {
  margin: 0%;
  color: rgb(153, 159, 164);
  transition: 0.4s;
}

.phone:hover {
  color: #f40057;
}

.github {
  width: 27px;
  transition: 0.4s;
  margin-top: 10px;
}
.github:hover {
  transform: scale(1.5);
}

.email {
  width: 60px;
  padding: 10px;
  transition: 0.4s;
  border-radius: 50%;
}
.email:hover {
  background: silver;
}
.phon {
  width: 50px;
  padding: 10px;
  transition: 0.4s;
  border-radius: 50%;
}
.phon:hover {
  background: silver;
}
.ending {
  width: 100%;
  height: 200px;
  background-color: rgb(38, 37, 37);
  margin-top: 80px;
}
/*////////////////////////🧑‍💻🧑‍💻🧑‍💻 responsive///////////// */
@media (max-width: 700px) {
  .github {
    width: 6%;
    margin-top: 0%;
  }

  .title {
    font-size: 28px;
  }
  .divTit {
    margin-left: 24%;
  }
  .aaa {
    font-size: 10px;
    font-weight: bold;
  }
  #word {
    display: none;
  }
  .tech {
    font-size: 10px;
    font-weight: bold;
  }
  .divTit {
    margin-left: 19%;
  }
  .laptop {
    // display: flex;
    width: 300px;

    height: 150px;
    width: 150px;
    // margin-top: 50px;
  }
  .me {
    margin-top: 35px;
    margin-left: 10px;
    font-size: 15px;
  }
  #about {
    flex-wrap: wrap;
    flex-direction: column;
    justify-content: center;
    margin-right: 40%;
  }

  #box {
    width: 300px;
    height: 250px;
    background: url(/3815805.jpg);
    background-position: center;
    background-size: cover;
    margin: 7% auto 30px; /* Centers horizontally */
    margin-top: 80px;
  }

  .amm {
    font-size: 10px;
    font-weight: bold;
    margin-top: 0%;
  }

  .airsheet {
    width: 90%;

    margin-left: 15px;
  }
  .mee {
    margin-left: 20px;
    margin-bottom: 5px;
    margin-top: 30px;
  }
  .mail {
    margin-left: 30px;
    display: flex;
  }
  .phone {
    margin-left: 5px;
    margin-top: 6px;
  }
  .contact {
    height: 230px;
  }
  .project {
    height: 400px;
  }
  .progress {
    width: 300px;
  }
}

// borderstyling//

.box {
  width: 400px;
  height: 300px;
  background: url(/3815805.jpg);
  background-position: center;
  background-size: cover;
  position: relative;
  box-shadow: 10px 10px 42px 0 rgba(0, 0, 0, 0.75);
  margin-top: 7%;
  margin-left: 37%;
  margin-bottom: 30px;
}
.box:after,
.box:before {
  mix-blend-mode: multiply;
  filter: none;
  z-index: -1;
  content: "";
  width: calc(100% + (50px * 2));
  height: calc(100% + (50px * 2));
  position: absolute;
  display: block;
  animation: border 10s ease-in-out infinite;
  transform: translateX(-50px) translateY(-50px);
}
@keyframes border {
  0%,
  100% {
    -webkit-clip-path: polygon(
      0 0,
      calc(100% - (33.3333333333px)) calc(0% + (33.3333333333px)),
      100% 100%,
      calc(0% + (33.3333333333px)) calc(100% - (33.3333333333px))
    );
    clip-path: polygon(
      0 0,
      calc(100% - (33.3333333333px)) calc(0% + (33.3333333333px)),
      100% 100%,
      calc(0% + (33.3333333333px)) calc(100% - (33.3333333333px))
    );
  }
  50% {
    -webkit-clip-path: polygon(
      calc(0% + (33.3333333333px)) calc(0% + (33.3333333333px)),
      100% 0,
      calc(100% - (33.3333333333px)) calc(100% - (33.3333333333px)),
      0 100%
    );
    clip-path: polygon(
      calc(0% + (33.3333333333px)) calc(0% + (33.3333333333px)),
      100% 0,
      calc(100% - (33.3333333333px)) calc(100% - (33.3333333333px)),
      0 100%
    );
  }
}

.box:after {
  animation-delay: -5s;
  background-color: #5995eb;
  clip-path: polygon(
    0 0,
    calc(100% - (33.3333333333px)) calc(0% + (33.3333333333px)),
    100% 100%,
    calc(0% + (33.3333333333px)) calc(100% - (33.3333333333px))
  );
}
.box:before {
  background-color: #f40057;
  clip-path: polygon(
    calc(0% + (33.3333333333px)) calc(0% + (33.3333333333px)),
    100% 0,
    calc(100% - (33.3333333333px)) calc(100% - (33.3333333333px)),
    0 100%
  );
}

// .box:hover:after {
//   animation-delay: -0.1s;
// }
// .box:hover:before,
// .box:hover:after {
//   animation-duration: 0.2s;
// }
</style>
