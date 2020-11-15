<template>
  <v-footer dark padless class="footer">
    <v-card class="flex" flat>
      <v-card-title>
        <v-spacer></v-spacer>

        <v-btn v-for="el in icons" :key="el.id" class="mx-2" icon>
          <a :href="el.url" target="_blank">
            <v-icon size="30px">
              {{ el.icon }}
            </v-icon>
          </a>
        </v-btn>
      </v-card-title>

      <v-card-text class="py-2 white--text text-center text-footer">
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
.footer a {
  color: white !important;
  text-decoration: none;
}
.footer .v-card__title {
  background-color: #262828;
}
.footer .text-footer {
  letter-spacing: 2.5px;
}
</style>