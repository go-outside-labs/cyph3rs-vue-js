<template>
  <div className="flex flex-col min-h-screen overflow-hidden">

    <!-- Site header -->
    <Header />

    <!-- Page content -->
    <main class="grow">

      <CareersText />

    </main>

    <!-- Site footer -->
    <Footer />

  </div>
</template>

<script>
import Header from '../partials/Header.vue'
import CareersText from '../partials/CareersText.vue'
import Footer from '../partials/Footer.vue'

export default {
  name: 'Careers',
  props: ['title'],
  watch: {
    title: {
      immediate: true,
      handler() {
        document.title = 'Careers - Cyph3rs';
      }
    }
  },
  render() {
  },
  components: {
    Header,
    CareersText,
    Footer,
  },
}
</script>