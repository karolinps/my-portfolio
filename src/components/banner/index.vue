<template>
  <v-parallax dark src="../../assets/images/back.jpg">
    <v-row align="center" justify="center">
      <v-col class="text-center" cols="12">
        <h1>Hola, soy Karolin Porras!</h1>
        <h4>Developer Frontend.</h4>
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
</style>