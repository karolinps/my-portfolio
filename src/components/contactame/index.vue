<template>
  <v-parallax dark src="../../assets/images/back.jpg" id="contactame">
    <h1>
      ¡Hola de nuevo, si quieres que trabajemos juntos, puedes contáctarme!
    </h1>
    <p><v-icon>mdi-email</v-icon> <span>porrask92@gmail.com</span></p>
    <p><v-icon>mdi-phone</v-icon> <span>(+51) 980219592</span></p>
  </v-parallax>
</template>

<script>
export default {
  name: "Contactame",
};
</script>

<style>
#contactame p {
  text-align: center;
}
#contactame h1 {
  margin-bottom: 15px;
}
#contactame .v-icon {
  color: white;
  margin-right: 4px;
}
#contactame span {
  font-size: 18px;
  letter-spacing: 1.5px;
}
</style>