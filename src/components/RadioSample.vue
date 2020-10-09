<template>
  <v-container>
    <v-row class="text-center">
      <div v-for="n in 3" :key="n">
        {{ `radioGroup${n}` }}
        <v-col cols="12">
          <v-radio-group :v-model="`radioGroup${n}`" :mandatory="false">
            <v-radio :label="`Chicago Bulls ${n}`" :value="`Bulls ${n}`"></v-radio>
            <v-radio :label="`Houston Rockets ${n}`" :value="`Rockets ${n}`"></v-radio>
          </v-radio-group>
        </v-col>
        <v-btn :disabled="`radioGroup${n}`">Click</v-btn>
      </div>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      radioGroup: false,
    };
  },
};
</script>
