<template>
  <footer class="footer">
    <Container>
      <div class="footer-items">
        <Logo />
        <FooterLinks />
        <SocialLinks />
      </div>

      <p><span>2022 © EmpireBurger.</span> Todos os direitos reservados.</p>
    </Container>
  </footer>
</template>

<style lang="scss" scoped>
.footer {
  background: rgba(59, 32, 11, 0.05);
  padding-block: 2rem;
  .container {
    height: 100%;
    display: grid;
    grid-template-columns: 1fr;
    grid-template-rows: auto;

    align-items: center;
    justify-content: center;

    > p {
      border-top: 0.3px solid #f3f3f3;
      padding-top: 2rem;

      text-align: center;

      span {
        font-weight: bold;
      }
    }

    .footer-items {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      padding-bottom: 2rem;

      .footer-links,
      .social-links {
        height: 100%;
        display: flex;
        align-items: center;
      }

      .footer-links {
        display: flex;
        gap: 1rem;
      }
    }
  }
}
</style>
