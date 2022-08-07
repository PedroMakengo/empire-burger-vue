<template>
  <header class="header">
    <Container>
      <Logo />
      <Navegator />
      <IfoodContact />
    </Container>
  </header>
</template>

<style lang="scss" scoped>
.header {
  background: rgba(59, 32, 11, 0.05);
  height: 10vh;

  .container {
    height: 100%;
    display: grid;
    grid-template-columns: 300px 1fr 300px;
    justify-content: center;
    align-items: center;
  }
}
</style>
