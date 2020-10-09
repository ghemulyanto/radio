<template>
  <v-app>
    <v-main>
      <RadioSample />
    </v-main>
  </v-app>
</template>

<script>
import RadioSample from "./components/RadioSample";

export default {
  name: "App",

  components: {
    RadioSample,
  },

  data: () => ({
    //
  }),
};
</script>
