<!-- GRANDE CONTENITORE IN CUI VERRANNO INSERITI UNO AD UNO TUTTTI I COMPONENTI -->
<script>
// COME IMPORTARE COMPONENTI IMPORT - NOME - FROM - PERCORSO
import AppContent1 from './components/AppContent1.vue';
import AppContent2 from './components/AppContent2.vue'
import AppContent3 from './components/AppContent3.vue';
import AppContentCarousel from './components/AppContentCarousel.vue';
import AppFooter from './components/AppFooter.vue';
import AppFooterCarousel from './components/AppFooterCarousel.vue';
import AppHeader from './components/AppHeader.vue';
import PartnersSection from './components/PartnersSection.vue';
import FixedLinks from './components/FixedLinks.vue'

// SCRIPT
export default {
  // QUA DICHIARO I COMPONENTI IMPORTATI
  components: {
    // ESEMPIO DI INPORT COMPONENTE
    AppHeader,
    AppContent1,
    AppContent2,
    AppContent3,
    AppContentCarousel,
    PartnersSection,
    AppFooterCarousel,
    FixedLinks,
    AppFooter,
  },
  data() {
    return {

    }
  },
  methods: {
    //PER PRENDERE FILE DA ASSETS
    getImg(path) {
      let risultato = new URL("../assets/img/" + path, import.meta.url);
      return risultato.href;
    },
  },
  mounted() {

  },
}
</script>

<template>
  <!-- TEMPLATE html-->
  <AppHeader />
  <AppContent1 />
  <AppContent2 />
  <div class="container">
    <AppContent3 />
    <AppContentCarousel />
  </div>
  <PartnersSection />
  <AppFooterCarousel />
  <!-- <div class="container">
    <CaroselloFooter />
  </div> -->
  <AppFooter />
  <FixedLinks />

</template>

<style>
/* STILE */
.container {
  width: 1200px;
  margin: 0 auto;
}
</style>
