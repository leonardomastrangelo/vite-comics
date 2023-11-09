<template>
  <HeaderDC />

  <main>
    <MainDC />
    <SectionDC />
  </main>

  <footer>
    footer
  </footer>
</template>

<script>
// components
import HeaderDC from './components/HeaderDC.vue';
import MainDC from './components/MainDC.vue';
import SectionDC from './components/SectionDC.vue';
export default {
  name: "App",
  components: {
    HeaderDC,
    MainDC,
    SectionDC,
  },
  data() {
    return {}
  },
  methods: {},
}
</script>

<style lang="scss"></style>