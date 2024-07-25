<template>
    <section class="py-16">
      <div class="text-center mb-16">
        <h2 class="text-3xl font-bold mb-4">Keep track of your snippets</h2>
        <p class="text-lg">Clipboard instantly stores any item you copy in the cloud, meaning you can access your snippets immediately on all your devices. Our Mac and iOS apps will help you organize everything.</p>
      </div>
      <v-row>
        <v-col cols="12" md="6">
          <v-img src="~/assets/images/image-computer.png" contain max-height="400" />
        </v-col>
        <v-col cols="12" md="6">
          <div class="space-y-8">
            <div v-for="(feature, index) in features" :key="index">
              <h3 class="text-xl font-bold mb-2">{{ feature.title }}</h3>
              <p>{{ feature.description }}</p>
            </div>
          </div>
        </v-col>
      </v-row>
    </section>
  </template>
  
  <script>
  export default {
    name: 'FeaturesSection',
    data: () => ({
      features: [
        { title: 'Quick Search', description: 'Easily search your snippets by content, category, web address, application, and more.' },
        { title: 'iCloud Sync', description: 'Instantly saves and syncs snippets across all your devices.' },
        { title: 'Complete History', description: 'Retrieve any snippets from the first moment you started using the app.' },
      ],
    }),
  }
  </script>