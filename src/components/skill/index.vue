<template>
  <v-parallax dark src="../../assets/images/back.jpg" id="skill">
    <h1>Mis Skills</h1>
    <v-row no-gutters>
      <v-col
        v-for="item in skills"
        v-bind:key="item.id"
        lg="2"
        md="2"
        sm="3"
        cols="6"
      >
        <v-card class="pa-2" outlined tile> {{ item.title }} </v-card>
      </v-col>
    </v-row>
  </v-parallax>
</template>

<script>
export default {
  name: "Skill",
  data() {
    return {
      skills: [
        {
          id: 1,
          title: "HTML5",
        },
        {
          id: 2,
          title: "CSS3",
        },
        {
          id: 3,
          title: "JS",
        },
        {
          id: 4,
          title: "LESS",
        },
        {
          id: 5,
          title: "React.js",
        },
        {
          id: 6,
          title: "Vue.js",
        },
        {
          id: 7,
          title: "Bootstrap",
        },
        {
          id: 8,
          title: "Material-UI",
        },
        {
          id: 9,
          title: "Ant Design",
        },
        {
          id: 10,
          title: "Vuetify",
        },
        {
          id: 11,
          title: "Node.js",
        },
        {
          id: 12,
          title: "Express.js",
        },
        {
          id: 13,
          title: "MongoDB",
        },
        {
          id: 14,
          title: "GitHub",
        },
        {
          id: 15,
          title: "GitLab",
        },
        {
          id: 16,
          title: "Bitbucket",
        },
        {
          id: 17,
          title: "Jira",
        },
        {
          id: 18,
          title: "Trello",
        },
        {
          id: 19,
          title: "VSC",
        },
        {
          id: 20,
          title: "Sublime Text",
        },
        {
          id: 21,
          title: "Ubuntu",
        },
        {
          id: 22,
          title: "Windows 10",
        },
      ],
    };
  },
};
</script>

<style>
#skill h1 {
  text-align: center;
  font-family: "Montserrat";
  font-size: 40px;
  letter-spacing: 0.5px;
  margin-top: 45px;
  margin-bottom: 25px;
}
#skill .v-parallax__content {
  height: auto !important;
}
#skill .v-card {
  text-align: center;
  letter-spacing: 1.5px;
  color: gray;
  font-weight: bold;
  border: 1px solid;
  margin-right: 10px;
  background: transparent;
  margin-bottom: 10px;
}
@media (max-width: 600px) {
  #skill {
    height: 800px !important;
  }
}
</style>