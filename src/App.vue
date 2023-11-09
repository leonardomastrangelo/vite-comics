<template>
  <HeaderDC />

  <main>
    <MainDC />
    <SectionDC />
  </main>

  <footer>
    <UpFooterDC />
  </footer>
</template>

<script>
// components
import HeaderDC from './components/HeaderDC.vue';
import MainDC from './components/MainDC.vue';
import SectionDC from './components/SectionDC.vue';
import UpFooterDC from './components/UpFooterDC.vue';
export default {
  name: "App",
  components: {
    HeaderDC,
    MainDC,
    SectionDC,
    UpFooterDC
  },
  data() {
    return {}
  },
  methods: {},
}
</script>

<style lang="scss"></style>