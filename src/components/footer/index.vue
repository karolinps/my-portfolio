<template>
  <v-footer dark padless class="footer">
    <v-card class="flex" flat>
      <v-card-title>
        <v-spacer></v-spacer>

        <v-btn v-for="el in icons" :key="el" class="mx-2" icon>
          <a :href="el.url" target="_blank">
            <v-icon size="30px">
              {{ el.icon }}
            </v-icon>
          </a>
        </v-btn>
      </v-card-title>

      <v-card-text class="py-2 white--text text-center">
        <strong>Karolin APS</strong> — {{ new Date().getFullYear() }}
      </v-card-text>
    </v-card>
  </v-footer>
</template>

<script>
export default {
  name: "Footer",
  data: () => ({
    icons: [
      { icon: "mdi-facebook", url: "https://www.facebook.com/karolindev" },
      {
        icon: "mdi-linkedin",
        url: "https://www.linkedin.com/in/karolin-porras",
      },
      { icon: "mdi-instagram", url: "https://www.instagram.com/karolindev" },
      { icon: "mdi-github", url: "https://www.github.com/karolinps" },
      { icon: "mdi-telegram", url: "https://t.me/karolindev" },
    ],
  }),
};
</script>

<style>
.footer a {
  color: white !important;
  text-decoration: none;
}
.footer .v-card__title {
  background-color: #262828;
}
</style>