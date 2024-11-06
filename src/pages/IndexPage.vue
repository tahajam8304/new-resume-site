<template>
  <q-page class="flex flex">
    <img class="image" src="/3815805.jpg" alt="coding" />
    <div class="divTit">
      <h2 class="title">Front-End Developer👋🏻</h2>
      <h5 class="aaa" style="margin-bottom: 0%">
        Hi, I'm Taha Jamalizade.A passionate Front-end Developer <br />
        based in Qom & Tehran. 📍
      </h5>
      <a target="_blank" href="https://github.com/tahajam8304">
        <img
          style="margin-bottom: 4%"
          class="github"
          src="/github-mark.svg"
          alt=""
        />
      </a>
      <div style="display: flex">
        <h6 class="tech" style="margin: 0%">Tech Stack |</h6>
        <img class="html" src="/icons8-html.svg" alt="html" />
        <img
          style="margin-left: 1%"
          class="html"
          src="/icons8-css.svg"
          alt="css"
        />
        <img class="html" src="/icons8-javascript.svg" alt="javascript" />
        <img
          style="margin-left: 3%"
          class="html"
          src="/icons8-vuejs.svg"
          alt="vue"
        />
        <img
          style="margin-left: 3px"
          class="html"
          src="/quasar-svgrepo-com.svg"
          alt="quasar"
        />
      </div>
      <br />
      <div id="about" style="display: flex; margin-top: 40px">
        <img class="laptop" src="/photolap.jpg" alt="laptop" />
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
    </div>
    <div id="projects" class="project">
      <h5 class="protit">(Projects)</h5>
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
        <h5 style="margin: 0%" class="title">Phone:</h5>
        <h6 class="phone">+989059229400</h6>
      </div>
      <div class="mail" style="margin-top: 3%">
        <img class="email" src="/email-1-svgrepo-com.svg" alt="" />
        <h5 style="margin: 0%" class="title">Mail:</h5>
        <a class="phone">mohammad.taha.jam@gmail.com</a>
      </div>
    </div>

    <div class="ending"></div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "IndexPage",
});
</script>

<style lang="scss">
.body--dark {
  .project {
    background-color: rgb(42, 41, 41);
  }
  .link {
    color: white;
  }
}

body {
  background-color: rgb(233, 232, 232);
}

.image {
  width: 30%;
  height: 20%;
  border-radius: 50%;
  border: black solid 5px;
  margin-top: 4%;
  margin-left: 37%;
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
  color: rgb(200, 25, 174);
  margin-bottom: 0%;
  margin-left: 40px;
}

.laptop {
  /* border: solid 2px black; */
  border-radius: 10%;
  padding: 1px;
  width: 20%;
  /* height: 40%; */
}

.project {
  width: 100%;
  height: 450px;
  background-color: rgb(222, 220, 220);
  display: grid;
  justify-content: center;
  margin-top: 4%;
}
.protit {
  font-weight: bold;
  margin-left: 220px;
  color: rgb(200, 25, 174);
  margin-top: 2px;
}

.airsheet {
  width: 500px;
  height: fit-content;
  margin-top: 20px;
  padding: 5px;
  margin-left: 40px;
  border: rgb(158, 155, 155) solid 3px;
  border-radius: 10px;
  margin-bottom: 0%;
  transition: 0.4s;
}

.link {
  color: black;
  text-decoration: none;
  margin-top: 0%;
  font-weight: bold;
  display: flex;
  justify-content: center;
  transition: 0.4s;
}
.link:hover {
  color: rgb(200, 25, 174);
}
.por {
  color: black;
  font-weight: bold;
  margin-top: 12%;
  font-size: x-large;
}
.mee {
  font-weight: bold;
  color: rgb(200, 25, 174);
  margin-left: 19%;
  margin-top: 6%;
}
.contact {
  width: 100%;
  height: 400px;
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
  color: rgb(200, 25, 174);
}

.github {
  width: 2%;
  transition: 0.4s;
}
.github:hover {
  transform: scale(1.5);
}

.email {
  width: 60px;
  padding: 10px;
}
.phon {
  width: 50px;
  padding: 10px;
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
  }
  .image {
    width: 40%;
    margin-left: 30%;
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
  .tech {
    font-size: 11px;
    font-weight: bold;
  }
  .divTit {
    margin-left: 19%;
  }
  .laptop {
    height: 150px;
    width: 150px;
    margin-top: 50px;
  }
  .me {
    margin-top: 35px;
    margin-left: 10px;
    font-size: 15px;
  }
  .amm {
    font-size: 10px;
    font-weight: bold;
    margin-top: 0%;
  }
  .protit {
    margin-left: 160px;
  }
  .airsheet {
    width: 100%;
    margin-left: 0%;
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
}
</style>
