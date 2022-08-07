<template>
  <div class="ifood-contact">
    <NuxtLink to="/">
      <img src="@/assets/img/ifood.svg" alt="Logo da Ifood" />
    </NuxtLink>
    <a href="/">
      <img src="@/assets/img/instagram-brands.svg" alt="Nosso instagram" />
    </a>
    <button>
      <img src="@/assets/img/whatsapp-brands.svg" alt="Nosso whatsapp" />
      Contato
    </button>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style lang="scss" scoped>
.ifood-contact {
  display: flex;
  align-items: center;

  button {
    display: flex;
    align-items: center;
    justify-content: center;

    background: color('secondary', 'base');
    width: 123px;
    height: 34px;

    border-radius: 4px;
    font-weight: 400;

    img {
      margin-right: 0.5rem;
    }

    &:hover {
      cursor: pointer;
      background: color('secondary', 'base');
    }
  }
}
</style>
