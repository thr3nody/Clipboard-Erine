<template>
  <v-app>
    <v-main>
      <v-container fluid class="pa-0">
        <header-section />
        <features-section />
        <devices-section />
        <workflow-section />
        <partners-section />
        <download-section />
        <footer-section />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import HeaderSection from '../components/HeaderSection.vue'
import FeaturesSection from '../components/FeaturesSection.vue'
import DevicesSection from '../components/DevicesSection.vue'
import WorkflowSection from '../components/WorkflowSection.vue'
import PartnersSection from '../components/PartnersSection.vue'
import DownloadSection from '../components/DownloadSection.vue'
import FooterSection from '../components/FooterSection.vue'

export default {
  name: 'MainPage',
  components: {
    HeaderSection,
    FeaturesSection,
    DevicesSection,
    WorkflowSection,
    PartnersSection,
    DownloadSection,
    FooterSection,
  },
}
</script>