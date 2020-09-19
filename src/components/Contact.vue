<template>
  <section id="contato" class="container">
    <div class="contact-info">
      <h2 class="title">
        Mande um oi para nós,
        <br />vamos criar juntos
      </h2>
      <p>Entre em contato conosco, e bata um papo para criarmos juntos uma WEB mais inteligente e conectada.</p>
      <a href="mailto:oi@progmar.dev" class="character-style-title">oi@progmar.dev</a>
    </div>
    <img src="../assets/illustrations/contact.svg" alt="Progmar :: Contact" />
  </section>
</template>

<script>
export default {
  name: "Contact",
};
</script>

<style lang="scss">
#contato {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  padding: 25px 0;

  .contact-info {
    & > p {
      margin-left: 15px;
      margin-bottom: 15px;
      width: 100%;
      max-width: 240px;
    }

    & > a {
      margin-left: 15px;

      &:hover {
        padding-bottom: 10px;
        border-bottom: 4px solid var(--color-secondary);
      }
    }
  }
}
</style>