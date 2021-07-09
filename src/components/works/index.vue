<template>
  <v-container id="works">
    <h1>Trabajos</h1>
    <v-row no-gutters>
      <v-col
        md="3"
        lg="3"
        sm="4"
        cols="12"
        v-for="work in works"
        :key="work.name"
      >
        <v-card dark>
          <v-card-title>
            <v-icon large left> mdi-domain </v-icon>
            <span class="">{{ work.name }}</span>
          </v-card-title>

          <v-card-text class="date">
            {{ work.date_begin }} - {{ work.date_end }}
          </v-card-text>
          <v-card-text class="description">
            {{ work.description }}
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "Works",
  data: () => ({
    works: [
      {
        name: "Sistelnet",
        date_begin: "Abril 2015",
        date_end: "Mayo 2016",
        description: "Desarrollo de un sistema de administración y gestión.",
      },
      {
        name: "Lince Solutions",
        date_begin: "Mayo 2016",
        date_end: "Julio 2016",
        description: "Creación de páginas, landing pages.",
      },
      {
        name: "Zippytech",
        date_begin: "Julio 2016",
        date_end: "Junio 2017",
        description:
          "Administración de página web, sistemas administrativos, catálago versión Netflix.",
      },
      {
        name: "Freelancer",
        date_begin: "Julio 2017",
        date_end: "Junio 2019",
        description: "Web site, one pages, CMS, plataforma virtual.",
      },
      {
        name: "Senda TI Solutions",
        date_begin: "Junio 2019",
        date_end: "Abril 2020",
        description: "App web de facturación electrónica.",
      },
      {
        name: "Altimea",
        date_begin: "Abril 2020",
        date_end: "Julio 2020",
        description: "Administrador catálogo digital.",
      },
      {
        name: "Freelancer",
        date_begin: "Julio 2020",
        date_end: "Actualidad",
        description: `Aplicación web intuitiva para ciclos PDCA,
          Aplicación web de operaciones,
          Calendario académico.`,
      },
    ],
  }),
};
</script>

<style>
#works {
  margin-bottom: 20px;
}
#works h1 {
  text-align: center;
  margin-bottom: 35px;
  font-family: "Montserrat";
  font-size: 40px;
  letter-spacing: 0.5px;
  margin-top: 20px;
}
#works .v-card {
  margin-bottom: 12px;
  height: 220px;
  margin-right: 10px !important;
  background-color: gray;
}
#works .description {
  font-size: 15px;
  letter-spacing: 0.5px;
  padding: 0px 13px;
}
#works .date {
  font-size: 15px;
  letter-spacing: 0.5px;
}
#works span {
  letter-spacing: 1.5px;
}
@media (max-width: 600px) {
  #works span {
    letter-spacing: 0.5px;
  }
}
</style>
