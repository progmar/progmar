<template>
  <footer>
    <div class="container character-style-footer">
      <div class="rights">
        <router-link to="/">
          <img src="../assets/logo-inverter.svg" alt="Progmar" />
        </router-link>
        <p>© Progmar Technologies.</p>
        <p>Todos os direitos reservados.</p>
      </div>
      <div class="socials">
        <a href="http://instagram.com/progmartech" target="_blank" rel="noopener noreferrer">
          <img src="../assets/icons/instagram.svg" alt="Progmar :: Instagram" />
        </a>
        <a href="http://linkedin.com/company/progmartech" target="_blank" rel="noopener noreferrer">
          <img src="../assets/icons/linkedin.svg" alt="Progmar :: LinkedIn" />
        </a>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "TheFooter",
};
</script>

<style lang="scss">
footer {
  background-color: var(--color-primary);
  padding: 50px 0;
  max-height: 200px;

  & > div {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
  }

  .rights img {
    margin-bottom: 15px;
  }

  .socials a:not(:last-of-type) {
    margin-right: 15px;
  }
}
</style>