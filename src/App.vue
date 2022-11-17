<template>
  <Navbar />
  <Header />
  <Footer />
</template>

<script>
import { defineComponent } from 'vue'
import Navbar from '@/components/Navbar'
import Header from '@/components/Header'
import Footer from '@/components/Footer'

export default defineComponent({
  name: 'App',

  components: {
    Navbar,
    Header,
    Footer,
  },
})
</script>
