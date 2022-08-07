<template>
  <NuxtLink to="/" class="logo">
    <img src="@/assets/img/logo.svg" alt="" />
    <h2>Empire <span>Burger</span></h2>
  </NuxtLink>
</template>

<style lang="scss" scoped>
.logo {
  display: grid;
  grid-template-columns: 25px 1fr;
  grid-gap: 0.5rem;

  align-items: center;
  justify-content: center;

  img {
    width: 100%;
  }
  h2 {
    font-weight: bold;
    text-transform: uppercase;
    color: rgba(29, 6, 5, 0.9);
    span {
      font-weight: 300;
    }
  }
}
</style>
