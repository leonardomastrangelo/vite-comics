<template>
  <HeaderDC />

  <main>
    <ContentDC />
  </main>

  <footer>
    footer
  </footer>
</template>

<script>
// components
import HeaderDC from './components/HeaderDC.vue';
import ContentDC from './components/ContentDC.vue';
export default {
  name: "App",
  components: {
    HeaderDC,
    ContentDC
  },
  data() { },
  methods: {},
}
</script>

<style lang="scss"></style>