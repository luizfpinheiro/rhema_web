<template>
  <v-row justify="center">
    <v-btn bottom text @click="dialog = true ? !dialog : true">AGENDA</v-btn>

    <v-dialog v-model="dialog" fullscreen hide-overlay transition="dialog-bottom-transition" max-width="290">
      <v-card>
        <v-card-title class="headline">Use Google's location service?</v-card-title>

        <v-card-text>Let Google help apps determine location. This means sending anonymous location data to Google, even when no apps are running.</v-card-text>

        <v-card-actions>
          <div class="flex-grow-1"></div>
        </v-card-actions>
      </v-card>
    </v-dialog>
  </v-row>
</template>

<script>
export default {
  data: () => ({
    "dialog": false
  }),
};
</script>
