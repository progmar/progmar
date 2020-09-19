<template>
  <header class="container">
    <router-link to="/">
      <img src="../assets/brand.svg" alt="Progmar" />
    </router-link>
    <nav>
      <router-link :to="{hash: '#o-que-fazemos'}" @click.passive="anchorHash">O que fazemos</router-link>
      <router-link :to="{hash: '#quem-somos'}" @click.passive="anchorHash">Quem Somos</router-link>
      <router-link :to="{hash: '#contato'}" @click.passive="anchorHash">Contato</router-link>
    </nav>
  </header>
</template>

<script>
export default {
  name: "TheHeader",
  methods: {
    anchorHash() {
      if (window.location.hash === this.$route.hash) {
        const el = document.getElementById(this.$route.hash.slice(1));
        if (el) {
          window.scrollTo({
            top: el.offsetTop,
            behavior: "smooth",
          });
        }
      }
    },
  },
  mounted() {
    this.anchorHash();
  },
};
</script>

<style lang="scss">
header {
  padding: 25px 0;
  max-height: 100px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;

  nav {
    a {
      font-family: var(--font-family-montserrat);
      font-style: var(--font-style-normal);
      font-weight: var(--font-weight-medium);
      font-size: var(--font-size-20);
      line-height: var(--line-spacing-2);
      color: var(--color-black);

      &:hover {
        padding-bottom: 10px;
        border-bottom: 4px solid var(--color-secondary);
      }

      &:not(:last-of-type) {
        margin-right: 15px;
      }
    }
  }
}
</style>