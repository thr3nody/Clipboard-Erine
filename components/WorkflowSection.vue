<template>
    <section class="text-center py-16">
      <h2 class="text-3xl font-bold mb-4">Supercharge your workflow</h2>
      <p class="text-lg mb-12">We've got the tools to boost your productivity.</p>
      <v-row justify="center">
        <v-col v-for="(feature, index) in features" :key="index" cols="12" sm="4" class="text-center">
          <v-img :src="feature.icon" contain height="50" class="mb-4 mx-auto" />
          <h3 class="text-xl font-bold mb-2">{{ feature.title }}</h3>
          <p>{{ feature.description }}</p>
        </v-col>
      </v-row>
    </section>
  </template>
  
  <script>
  export default {
    name: 'WorkflowSection',
    data: () => ({
      features: [
        { icon: '~/assets/images/icon-blacklist.svg', title: 'Create blacklists', description: 'Ensure sensitive information never makes its way to your clipboard by excluding certain sources.' },
        { icon: '~/assets/images/icon-text.svg', title: 'Plain text snippets', description: 'Remove unwanted formatting from copied text for a consistent look.' },
        { icon: '~/assets/images/icon-preview.svg', title: 'Sneak preview', description: 'Quick preview of all snippets on your Clipboard for easy access.' },
      ],
    }),
  }
  </script>