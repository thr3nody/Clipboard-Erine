<template>
    <section class="text-center py-16">
      <v-img :src="logo" alt="Logo" class="mx-auto mb-6" width="60" height="60" />
      <h1 class="text-4xl font-bold mb-4">A history of everything you copy</h1>
      <p class="text-lg mb-8">Clipboard allows you to track and organize everything you copy. Instantly access your clipboard on all your devices.</p>
      <div class="flex justify-center space-x-4">
        <v-btn color="teal" class="white--text">Download for iOS</v-btn>
        <v-btn color="indigo" class="white--text">Download for Mac</v-btn>
      </div>
    </section>
  </template>
  
  <script>
  import Logo from '~/assets/images/logo.svg'
  
  export default {
    name: 'HeaderSection',
    components: {
      Logo
    },
    data() {
        return {
            logo: require('~/assets/images/logo.svg')
        }
    },
  }
  </script>