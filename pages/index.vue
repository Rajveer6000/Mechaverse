<template>
  <div>
    <!-- <gallery /> -->
    <Footer />
    <Navbar />
  </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue';
import Footer from '~/components/footer.vue';

export default {
  name: 'IndexPage',
  components: { Footer, Navbar }
}
</script>
