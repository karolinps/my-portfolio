<template>
  <v-parallax dark src="../../assets/images/back.jpg" id="home">
    <v-row align="center" justify="center">
      <v-col class="text-center" cols="12">
        <h1>Hola, soy Karolin Porras!</h1>
        <h4>Desarrolladora Frontend.</h4>
        <v-btn v-for="el in icons" :key="el.id" class="mx-2" icon>
          <a :href="el.url" target="_blank">
            <v-icon>
              {{ el.icon }}
            </v-icon>
          </a>
        </v-btn>
      </v-col>
    </v-row>
  </v-parallax>
</template>

<script>
export default {
  name: "Banner",
  data: () => ({
    icons: [
      {
        id: 1,
        icon: "mdi-facebook",
        url: "https://www.facebook.com/karolindev",
      },
      {
        id: 2,
        icon: "mdi-linkedin",
        url: "https://www.linkedin.com/in/karolin-porras",
      },
      {
        id: 3,
        icon: "mdi-instagram",
        url: "https://www.instagram.com/karolindev",
      },
      { id: 4, icon: "mdi-github", url: "https://www.github.com/karolinps" },
      { id: 5, icon: "mdi-telegram", url: "https://t.me/karolindev" },
    ],
  }),
};
</script>

<style>
h1 {
  text-align: center;
  font-family: "Montserrat";
  font-size: 40px;
  letter-spacing: 0.5px;
}
h4 {
  text-align: center;
  font-family: "Montserrat";
  font-size: 20px;
  letter-spacing: 0.5px;
}
#home .v-icon {
  font-size: 30px;
  color: white;
  margin-right: 4px;
  margin-top: 10px;
  cursor: pointer;
}
#home a {
  color: white !important;
  text-decoration: none;
}
</style>