<template>
  <section id="performance" class="container">
    <img src="../assets/illustrations/performance.svg" alt="Progmar :: Performance" />
    <div class="performance-info">
      <h2 class="title">
        Desenvolvendo aplicações com
        <br />alto desempenho
      </h2>
      <p>A Progmar Technologies vem com uma missão, de tornar a WEB um lugar mais inteligente, desenvolvendo aplicações com alto desempenho e satisfação para seus clientes.</p>
    </div>
  </section>
</template>

<script>
export default {
  name: "Performance",
};
</script>

<style lang="scss">
#performance {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  padding: 25px 0;

  .performance-info {
    & > p {
      margin-left: 15px;
      margin-bottom: 15px;
      width: 100%;
      max-width: 330px;
    }
  }
}
</style>