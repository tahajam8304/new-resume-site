<template>
  <q-layout view="lHh Lpr lFf">
    <div class="header">
      <a href="#default" class="logo">Taha.Code</a>
      <div class="header-right">
        <a class="btn">Home</a>
        <!-- <button >About</button> -->
        <a class="btn" @click="goToAbout">About</a>
        <a class="btn" @click="gotoproject">Projects</a>
        <a class="btn" @click="gotocontact">Contact</a>
      </div>
    </div>
    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from "vue";
// import EssentialLink from "components/EssentialLink.vue";

const linksList = [];

export default defineComponent({
  name: "MainLayout",

  // components: {
  //   EssentialLink
  // },

  setup() {
    const leftDrawerOpen = ref(false);

    const goToAbout = () => {
      window.scrollTo({
        top: document.getElementById("about").offsetTop,
        left: 0,
        behavior: "smooth",
      });
    };

    const gotoproject = () => {
      window.scrollTo({
        top: document.getElementById("projects").offsetTop,
        left: 0,
        behavior: "smooth",
      });
    };

    const gotocontact = () => {
      window.scrollTo({
        top: document.getElementById("contact").offsetTop,
        left: 0,
        behavior: "smooth",
      });
    };
    /////////////////////////////////////////// dark mode script/////////////////////////////


    return {
      linksList,
      leftDrawerOpen,
      toggleLeftDrawer() {
        leftDrawerOpen.value = !leftDrawerOpen.value;
      },
      goToAbout,
      gotoproject,
      gotocontact,
    };
  },
});
</script>

<style>
.header {
  overflow: hidden;
  background-color: #ffffff;
  padding: 20px 10px;
}

/* Style the header links */
.header a {
  float: left;
  color: #000000;
  text-align: center;
  padding: 12px;
  text-decoration: none;
  font-size: 18px;
  line-height: 25px;
  border-radius: 4px;
  font-weight: bold;
  transition: 0.4s;
}

/* Style the logo link (notice that we set the same value of line-height and font-size to prevent the header to increase when the font gets bigger */
.header a.logo {
  font-size: 25px;
  font-weight: bold;
  padding-right: 30px;
}

/* Change the background color on mouse-over */
.header a:hover {
  /* background-color: #ddd; */
  color: rgb(195, 22, 204);
}

/* Style the active/current link*/
/* .header a.active {
  background-color: dodgerblue;
  color: white;
} */

/* Float the link section to the right */
.header-right {
  float: right;
}

/* Add media queries for responsiveness - when the screen is 500px wide or less, stack the links on top of each other */
@media screen and (max-width: 700px) {
  .header {
    padding-left: 0%;
  }
  .header a.logo {
    font-size: 20px;
    /* font-weight: normal; */
    padding: 0%;
  }
  .header a.btn {
    padding: 7px;
    padding-left: 2px;
  }
}
</style>
