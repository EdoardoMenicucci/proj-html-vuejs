<!-- GRANDE CONTENITORE IN CUI VERRANNO INSERITI UNO AD UNO TUTTTI I COMPONENTI -->
<script>
// COME IMPORTARE COMPONENTI IMPORT - NOME - FROM - PERCORSO
import AppContent1 from './components/AppContent1.vue';
import AppContent2 from './components/AppContent2.vue'
import AppContent3 from './components/AppContent3.vue';
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';

// SCRIPT
export default {
  // QUA DICHIARO I COMPONENTI IMPORTATI
  components: {
    // ESEMPIO DI INPORT COMPONENTE
    AppHeader,
    AppContent1,
    AppContent2,
    AppContent3,
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
  </div>
  <AppFooter />
</template>

<style>
/* STILE */
.container {
  width: 1200px;
  margin: 0 auto;
}
</style>
