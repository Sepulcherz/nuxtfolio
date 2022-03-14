<template>
  <div>
    <section class="section">
      <h1 class="aboutstyle2 title is-3 has-text-grey">
        If you have any questions or if you just wanna say hi,
        <br />
        feel free to contact me.
      </h1>
      <div class="columns is-mobile">
        <card title="Send me an e-mail!" icon="card-account-mail">
          <a href="mailto:mr_devaux@hotmail.fr"> mr_devaux@hotmail.fr </a>
        </card>
        <div class="section title is-3 has-text-grey">
          <p>or</p>
        </div>
        <card title="Send me a message on discord!" icon="card-account-phone">
          <p>Waster of oxygen™☕🚬⚰#3324</p>
        </card>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "Contact",
};
</script>

<style scoped>
@media only screen and (max-width: 500px) {
  .columns .is-mobile {
    flex-direction: column;
  }
  p {
    justify-content: center;
    align-items: center;
    text-align: center;
  }
} ;
</style>