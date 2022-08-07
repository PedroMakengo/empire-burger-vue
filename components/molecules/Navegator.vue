<template>
  <nav class="navegator">
    <ul>
      <li v-for="link of links" :key="link.id">
        <NuxtLink :to="link.to">{{ link.text }}</NuxtLink>
      </li>
    </ul>
  </nav>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data() {
    return {
      links: [
        { id: 1, to: '/', text: 'Home' },
        { id: 2, to: '/', text: 'Promoção' },
        { id: 3, to: '/', text: 'Cardápio' },
        { id: 4, to: '/', text: 'Comentário' },
        { id: 5, to: '/', text: 'Contato' },
      ],
    }
  },
})
</script>

<style lang="scss" scoped>
.navegator {
  ul {
    display: flex;
    gap: 1rem;

    li {
      a {
        text-decoration: none;
        color: color('text', 'title-87');
      }
    }
  }
}
</style>
