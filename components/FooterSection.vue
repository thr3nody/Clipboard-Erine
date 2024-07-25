<template>
    <footer class="bg-gray-100 py-8">
      <v-container>
        <v-row align="center">
          <v-col cols="12" md="2">
            <v-img src="~/assets/images/logo.svg" max-width="60" />
          </v-col>
          <v-col cols="12" md="8">
            <v-row>
              <v-col v-for="(link, index) in links" :key="index" cols="6" sm="4">
                <a href="#" class="text-gray-600 hover:text-gray-800">{{ link }}</a>
              </v-col>
            </v-row>
          </v-col>
          <v-col cols="12" md="2">
            <div class="flex justify-center md:justify-end space-x-4">
              <a v-for="(icon, index) in socialIcons" :key="index" href="#" class="text-gray-600 hover:text-gray-800">
                <v-icon>{{ icon }}</v-icon>
              </a>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </footer>
  </template>
  
  <script>
  export default {
    name: 'FooterSection',
    data: () => ({
      links: ['FAQs', 'Contact Us', 'Privacy Policy', 'Press Kit', 'Install Guide'],
      socialIcons: ['mdi-facebook', 'mdi-twitter', 'mdi-instagram'],
    }),
  }
  </script>