<template>
  <v-container id="about">
    <h1>Sobre mi</h1>
    <v-row no-gutters>
      <v-col md="4" sm="4" offset-md="2" offset-sm="2">
        <v-img src="../../assets/images/me.jpeg" />
      </v-col>
      <v-col md="4" sm="4" offset-md="1" offset-sm="1">
        <p>
          Mi nombre es Karolin Angelica Porras Serrano, tengo 27 años, soy
          Ingeniero de Sistemas, egresada en el 2015 de la UNEFA, nací en
          Venezuela, pero actualmente resido en Lima - Perú, desde que egrese
          empece a trabajar en el área de programación, pasando por varias
          empresas que me han permitido aportar, aprender y crecer
          profesionalmente. Trabajo en el área del frontend, pero he realizado
          algunos trabajo como backend.
        </p>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "About",
};
</script>

<style>
#about {
  margin-bottom: 30px;
}
#about h1 {
  text-align: center;
  margin-bottom: 35px;
  font-family: "Montserrat";
  font-size: 40px;
  letter-spacing: 0.5px;
  margin-top: 20px;
}
p {
  text-align: justify;
  font-family: "Roboto";
  line-height: 25px;
  letter-spacing: 0.5px;
  font-size: 15px;
}
@media(max-width: 600px){
  p {
    margin-top: 12px;
  }
}
</style>