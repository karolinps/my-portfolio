<template>
  <v-parallax dark src="../../assets/images/back.jpg" id="home">
    <v-row align="center" justify="center">
      <v-col class="text-center" cols="12">
        <h1>Hola, soy Karolin Porras!</h1>
        <h4>Desarrolladora Frontend.</h4>
        <a href="https://www.facebook.com/karolindev" target="_blank">
          <v-icon> mdi-facebook</v-icon>
        </a>
        <a href="https://www.linkedin.com/in/karolin-porras" target="_blank">
          <v-icon>mdi-linkedin</v-icon>
        </a>
        <a href="https://www.instagram.com/karolindev" target="_blank">
          <v-icon>mdi-instagram</v-icon>
        </a>
        <a href="https://www.github.com/karolinps" target="_blank">
          <v-icon>mdi-github</v-icon>
        </a>
        <a href="https://t.me/karolindev" target="_blank">
          <v-icon>mdi-telegram</v-icon>
        </a>
      </v-col>
    </v-row>
  </v-parallax>
</template>

<script>
export default {
  name: "Banner",
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
</style>