<template>
  <v-parallax
      :src="merchant.banner"
  >
    <v-col class="text-center">
      <v-img 
        width="180"
        class="mx-auto"
        :src="merchant.logo">
      </v-img>
      <h2>{{ merchant.slogan }}</h2>
      <h3>Ahora puedes pedir tu delivery cuando quieras!</h3>
    </v-col>
  </v-parallax>
</template>

<script>
export default {
  computed: {
    merchant() {
      return this.$store.state.merchant
    }
  },
}
</script>

<style scoped></style>