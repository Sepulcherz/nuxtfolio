<template>
  <div>
    <section class="section">
      <div class="columns is-mobile">
        <card title="Send me an e-mail!" icon="card-account-mail">
          <a href="mailto:mr_devaux@hotmail.fr"> mr_devaux@hotmail.fr </a>
        </card>
        <div class="section title is-3 has-text-grey">
          <p>or</p>
        </div>
        <card title="Send me a message on discord" icon="card-account-phone">
          *discord something something*
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
};
</style>
