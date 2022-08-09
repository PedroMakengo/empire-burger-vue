<template>
  <nav class="footer-links">
    <NuxtLink v-for="link of footerLinks" :key="link.id" :to="link.to">
      {{ link.text }}
    </NuxtLink>
  </nav>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data() {
    return {
      footerLinks: [
        { id: 1, to: '/', text: 'Home' },
        { id: 2, to: '/', text: 'Localização' },
        { id: 3, to: '/', text: 'Cardápio' },
        { id: 4, to: '/', text: 'Sobre' },
      ],
    }
  },
})
</script>

<style lang="scss" scoped>
.footer-links {
  a {
    font-weight: 400;
    color: #000;
  }
}
</style>
