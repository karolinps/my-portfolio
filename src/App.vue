<template>
  <v-app>
    <Header />
    <Banner />
    <About />
    <Skill />
    <Works />
    <Contactame />
    <v-main> </v-main>
  </v-app>
</template>
<script>
import Header from "./components/header/index";
import Banner from "./components/banner/index";
import About from "./components/about/index";
import Skill from "./components/skill/index";
import Works from "./components/works/index";
import Contactame from "./components/contactame/index";
export default {
  name: "App",

  components: {
    Header,
    Banner,
    About,
    Skill,
    Works,
    Contactame,
  },

  data: () => ({
    //
  }),
};
</script>
