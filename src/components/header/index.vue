 <template>
  <v-app-bar app class="app-bar">
    <div class="menu">
      <v-btn>
        <a href="#home"> <span>Inicio</span> </a>
      </v-btn>
      <v-btn>
        <a href="#about"> <span>Sobre mi</span> </a>
      </v-btn>
      <v-btn>
        <a href="#skill"> <span>Skills</span> </a>
      </v-btn>
      <v-btn>
        <a href="#works"> <span>Trabajo</span> </a>
      </v-btn>
      <v-btn>
        <a href="#contactame"> <span>Contáctame</span> </a>
      </v-btn>
    </div>
  </v-app-bar>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style>
.menu a {
  color: white !important;
  text-decoration: none;
}
</style>