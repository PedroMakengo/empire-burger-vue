<template>
  <div class="ifood-contact">
    <SocialLinks />
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
  justify-content: flex-end;

  .social-links {
    display: flex;
    justify-content: center;
    align-items: center;

    &:after {
      content: '';

      display: block;
      width: 1px;
      height: 3.2rem;
      background: #b50b04;
      margin-right: 5px;
    }
  }

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
