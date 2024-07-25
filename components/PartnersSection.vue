<template>
    <section class="py-16">
      <v-row justify="center" align="center">
        <v-col v-for="(partner, index) in partners" :key="index" cols="6" sm="4" md="2">
          <v-img :src="partner" contain height="50" />
        </v-col>
      </v-row>
    </section>
  </template>
  
  <script>
  export default {
    name: 'PartnersSection',
    data: () => ({
      partners: [
        '~/assets/images/logo-google.png',
        '~/assets/images/logo-ibm.png',
        '~/assets/images/logo-microsoft.png',
        '~/assets/images/logo-hp.png',
        '~/assets/images/logo-vector-graphics.png',
      ],
    }),
  }
  </script>