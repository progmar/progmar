<template>
  <section id="o-que-fazemos" class="container">
    <div class="welcome-info">
      <h1 class="title">
        Por uma WEB mais inteligente
        <br />e conectada
      </h1>
      <p>Bem vindos à Progmar Technologies, desenvolvendo ideais que conectam as pessoas. Qualidade, inteligência e colaboração.</p>
    </div>
    <img src="../assets/illustrations/welcome.svg" alt="Progmar :: Welcome" />
  </section>
</template>

<script>
export default {
  name: "Welcome",
};
</script>

<style lang="scss">
#o-que-fazemos {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: center;
  padding: 25px 0;

  .welcome-info {
    & > p {
      margin-left: 15px;
      margin-bottom: 15px;
      width: 100%;
      max-width: 327px;
    }
  }
}
</style>