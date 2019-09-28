<template>
  <v-row justify="center">
    <v-btn bottom text @click="dialog = true ? !dialog : true">AGENDA</v-btn>
    <v-dialog v-model="dialog" transition="dialog-bottom-transition" width="400">
      <v-card hover>
        <v-list-item>
          <v-list-item-content>
            <v-list-item-title class="title">Culto de Celebração</v-list-item-title>
            <v-list-item-subtitle class="subtitle-1 pa-2">Domingos - 19H</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>

        <v-list-item two-line>
          <v-list-item-content>
            <v-list-item-title class="title">Redes</v-list-item-title>
            <v-list-item-subtitle class="subtitle-1 pa-2">Sábados - 19:30H</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>

        <v-list-item three-line>
          <v-list-item-content>
            <v-list-item-title class="title">Escola Bíblica Discipular</v-list-item-title>
            <v-list-item-subtitle class="subtitle-1 pa-2">Quintas-Feiras - 20H</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
      </v-card>
    </v-dialog>
  </v-row>
</template>

<script>
export default {
  data: () => ({
    dialog: false,
    items: [
      {
        icon: "mdi-home",
        text: "DOMINGO - 19H"
      },
      {
        icon: "mdi-home",
        text: "SÁBADO - 19:30H"
      },
      {
        icon: "mdi-home",
        text: "QUINTA-FEIRA - 20H"
      }
    ],
    model: 1
  })
};
</script>
