<template>
  <Navbar />
  <Header />
</template>

<script>
import { defineComponent } from 'vue'
import Navbar from '@/components/Navbar'
import Header from '@/components/Header'

export default defineComponent({
  name: 'App',

  components: {
    Navbar,
    Header,
  },
})
</script>
