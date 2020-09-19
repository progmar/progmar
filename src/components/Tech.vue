<template>
  <section id="quem-somos" class="container">
    <div class="tech-info">
      <h2 class="title">
        Usando o que há de melhor,
        <br />para fazer o que há de melhor
      </h2>
      <p>Utilizamos as melhores linguagens para criarmos juntos o que há de melhor. Desbrave conosco com as melhores tecnologias.</p>
    </div>
    <div class="tech-langs">
      <div class="lang">
        <img src="../assets/langs/php.svg" alt="Progmar :: PHP" />
      </div>
      <div class="lang">
        <img src="../assets/langs/flutter.svg" alt="Progmar :: Flutter" />
      </div>
      <div class="lang">
        <img src="../assets/langs/vue.svg" alt="Progmar :: VueJs" />
      </div>
      <div class="lang">
        <img src="../assets/langs/react.svg" alt="Progmar :: React & React Native" />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Tech",
};
</script>

<style lang="scss">
#quem-somos {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: center;
  padding: 25px 0;

  .tech-info {
    & > p {
      margin-left: 15px;
      margin-bottom: 15px;
      width: 100%;
      max-width: 308px;
    }
  }

  .tech-langs {
    display: flex;
    flex-direction: row;

    & .lang {
      border-radius: 5px;
      background-color: var(--color-primary);
      height: 150px;
      width: 150px;
      display: flex;
      justify-content: center;
      align-items: center;

      &:not(:last-of-type) {
        margin-right: 15px;
      }
    }
  }
}
</style>