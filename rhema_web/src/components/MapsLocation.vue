<template>
  <v-content>
    <div class="mapouter">
      <div class="gmap_canvas">
        <iframe
          width="400"
          height="300"
          id="gmap_canvas"
          src="https://maps.google.com/maps?q=Rhema%20Minist%C3%A9rio%20Apost%C3%B3lico&t=&z=17&ie=UTF8&iwloc=&output=embed"
          frameborder="0"
          scrolling="no"
          marginheight="0"
          marginwidth="0"
        ></iframe>
      </div>
    </div>
  </v-content>
</template>

<script>
export default {
  data: () => ({})
};
</script>
