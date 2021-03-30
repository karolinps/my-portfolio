<template>
  <v-container id="projects">
    <v-divider></v-divider>
    <h1>Proyectos</h1>
    <v-row>
      <v-col
        v-for="card in projects"
        :key="card.title"
        sm="4"
        md="4"
        lg="4"
        cols="12"
      >
        <h5>{{ card.title }}</h5>
        <v-card>
          <a :href="card.url" target="_blank"
            ><v-img :src="card.src"> </v-img>
          </a>
        </v-card>
        <p
          style="font-size:14px; text-align: center;
font-weight: bold;"
        >
          {{ card.description }}
        </p>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import admin from "../../assets/images/admin_tikvao.png";
import calculadora from "../../assets/images/calculadora.png";
import pageGatsby from "../../assets/images/page-gatsby-translate.png";
import nextFirstProject from "../../assets/images/next-first-project.png";
import rickAndMortyRedux from "../../assets/images/rickandmorty.png";
import withFirebase from "../../assets/images/with-firebase.png";

export default {
  name: "Projects",
  data: () => ({
    projects: [
    {
        title: "CRUD con firebase",
        description:
          "Desarrollado con Reactjs, Ant Desing e Integración Firebase ",
        src: withFirebase,
        url: "https://crud-with-firebase.vercel.app/",
      },
      {
        title: "Aplicación Rick and Morty",
        description:
          "Desarrollado con Reactjs, Redux, Styled Components, consumiendo api externa de Rick and Morty",
        src: rickAndMortyRedux,
        url: "https://react-redux-rickandmorty.vercel.app/",
      },
      {
        title: "Aplicación listado de usuarios",
        description:
          "Desarrollado con Nextjs, consumiendo api externa y Ant Desing",
        src: nextFirstProject,
        url: "https://nextjs-first-project-iota.vercel.app/login",
      },
      {
        title: "Landing",
        description:
          "Desarrollado con Gatsby, integrando sistema de traducción y Ant Desing",
        src: pageGatsby,
        url: "https://page-gatsby-translate.vercel.app",
      },
      {
        title: "Administrador",
        description: "Desarrollado con Reactjs, Ant Desing, Nodejs y MongoDB",
        src: admin,
        url: "https://panel-administrator.netlify.app",
      },

      {
        title: "Calculadora de préstamos",
        description: "HTML, CSS & JS",
        src: calculadora,
        url: "https://mqyn8wr3mj.csb.app/",
      },
    ],
  }),
};
</script>

<style>
#projects {
  margin-bottom: 20px;
}
#projects h1 {
  text-align: center;
  margin-bottom: 35px;
  font-family: "Montserrat";
  font-size: 40px;
  letter-spacing: 0.5px;
  margin-top: 20px;
}
#projects h5 {
  font-family: "Montserrat";
  font-size: 18px;
  font-weight: bold;
  text-align: center;
  margin-bottom: 10px;
}
#projects .v-card {
  margin-bottom: 12px;
  height: 220px;
  margin-right: 10px !important;
  background-color: gray;
}
</style>
