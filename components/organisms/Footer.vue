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
  background: red;
  padding-block: 2rem;
  .container {
    height: 100%;
    display: grid;
    grid-template-columns: 1fr;
    grid-template-rows: auto;

    align-items: center;
    justify-content: center;

    > p {
      padding-top: 2rem;
      border-top: 0.3px solid #f3f3f3;

      text-align: center;

      color: #f7f7f7;
      span {
        font-weight: bold;
      }
    }

    .footer-items {
      display: grid;
      grid-template-columns: 1fr 1fr 100px;
      padding-bottom: 2rem;

      .footer-links,
      .social-links {
        height: 100%;
        display: flex;
        align-items: center;
      }

      .footer-links {
        display: flex;
        gap: 2rem;
      }

      .social-links {
        justify-content: flex-end;
        gap: 1rem;

        svg path,
        svg rect {
          fill: #000;
        }
      }
    }
  }
}
</style>
