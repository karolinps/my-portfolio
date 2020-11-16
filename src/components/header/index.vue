 <template>
  <v-app-bar app class="app-bar">
    <div class="menu hidden-sm-and-down">
      <v-btn v-for="item in menu" :key="item.href">
        <a :href="item.href">
          <span>{{ item.title }}</span>
        </a>
      </v-btn>
    </div>
    <v-app-bar-nav-icon
      @click="drawer = true"
      class="hidden-md-and-up icon-drawer"
    ></v-app-bar-nav-icon>
    <v-navigation-drawer v-model="drawer" absolute temporary>
      <v-list nav dense>
        <v-list-item-group
          v-for="item in menu"
          :key="item.href"
          active-class="deep-purple--text text--accent-4"
        >
          <v-list-item>
            <v-list-item-title
              ><a :href="item.href" @click="drawer = false">
                <span>{{ item.title }}</span>
              </a></v-list-item-title
            >
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </v-app-bar>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      drawer: false,
      menu: [
        { href: "#home", title: "Inicio" },
        { href: "#about", title: "Sobre mi" },
        { href: "#skill", title: "Skills" },
        { href: "#works", title: "Trabajo" },
        { href: "#projects", title: "Proyectos" },
        { href: "#contactame", title: "Conctáctame" },
      ],
    };
  },
};
</script>

<style>
.menu a {
  color: white !important;
  text-decoration: none;
}
.app-bar aside {
  height: 100vh !important;
}
.app-bar .v-list-item__title a {
  color: gray !important;
  text-decoration: none;
  font-size: 15px;
  letter-spacing: 0.5px;
}
.app-bar .icon-drawer {
  color: white !important;
}
</style>