<template>
  <section id="team" class="container">
    <div class="members">
      <div class="member">
        <img src="../assets/avatars/marcelo.png" alt="Marcelo Pecin" class="avatar" />
        <p>Marcelo Pecin | CTO</p>
        <div class="socials">
          <a href="http://instagram.com/celopeccin" target="_blank" rel="noopener noreferrer">
            <img src="../assets/icons/instagram-inverse.svg" alt="Marcelo Pecin :: Instagram" />
          </a>
          <a href="http://linkedin.com/in/celopeccin" target="_blank" rel="noopener noreferrer">
            <img src="../assets/icons/linkedin-inverse.svg" alt="Marcelo Pecin :: LinkedIn" />
          </a>
        </div>
      </div>
      <div class="member">
        <img src="../assets/avatars/giovana.jpeg" alt="Giovana Schnorr" class="avatar" />
        <p>Giovana Schnorr | Designer</p>
        <div class="socials">
          <a href="http://instagram.com/gischnorr" target="_blank" rel="noopener noreferrer">
            <img src="../assets/icons/instagram-inverse.svg" alt="Giovana Schnorr :: Instagram" />
          </a>
          <a href="http://linkedin.com/in/gioschnorr/" target="_blank" rel="noopener noreferrer">
            <img src="../assets/icons/linkedin-inverse.svg" alt="Giovana Schnorr :: LinkedIn" />
          </a>
        </div>
      </div>
      <div class="member">
        <img src="../assets/avatars/william.jpeg" alt="William David" class="avatar" />
        <p>William David | Developer</p>
        <div class="socials">
          <a href="http://instagram.com/williamd_cwb" target="_blank" rel="noopener noreferrer">
            <img src="../assets/icons/instagram-inverse.svg" alt="William David :: Instagram" />
          </a>
          <a
            href="http://linkedin.com/in/william-david-56a085b3/"
            target="_blank"
            rel="noopener noreferrer"
          >
            <img src="../assets/icons/linkedin-inverse.svg" alt="William David :: LinkedIn" />
          </a>
        </div>
      </div>
    </div>
    <div class="team-info">
      <h2 class="title">
        Junto com o melhor time para
        <br />criarmos e irmos sempre além
      </h2>
      <p>O melhor time de profissionais que estão sempre prontos para o desafio, e lhe ajudando na melhor solução. Tornando assim, uma WEB mais inteligente e conectada.</p>
    </div>
  </section>
</template>

<script>
export default {
  name: "Team",
};
</script>

<style lang="scss">
#team {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  padding: 25px 0;

  .team-info {
    & > p {
      margin-left: 15px;
      margin-bottom: 15px;
      width: 100%;
      max-width: 318px;
    }
  }

  .members {
    display: flex;
    flex-direction: row;
    align-items: center;

    & .member {
      display: flex;
      flex-direction: column;
      align-items: center;

      &:not(:last-of-type) {
        margin-right: 15px;
      }

      & .avatar {
        background-color: var(--color-primary);
        border: 4px solid var(--color-primary);
        border-radius: 100%;
        width: 208px;
        height: 208px;
        object-fit: cover;
        margin-bottom: 15px;
      }

      & p {
        margin-bottom: 15px;
      }

      & .socials a:not(:last-of-type) {
        margin-right: 10px;
      }
    }
  }
}
</style>