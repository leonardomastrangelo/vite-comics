<template>
  <HeaderDC />

  <main>
    <MainDC />
    <SectionDC />
  </main>

  <footer>
    <UpFooterDC />
    <DownFooter />
  </footer>
</template>

<script>
// components
import HeaderDC from './components/HeaderDC.vue';
import MainDC from './components/MainDC.vue';
import SectionDC from './components/SectionDC.vue';
import UpFooterDC from './components/UpFooterDC.vue';
import DownFooter from './components/DownFooterDc.vue'
export default {
  name: "App",
  components: {
    HeaderDC,
    MainDC,
    SectionDC,
    UpFooterDC,
    DownFooter
  },
  data() {
    return {}
  },
  methods: {},
}
</script>

<style lang="scss"></style>