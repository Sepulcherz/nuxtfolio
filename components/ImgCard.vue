<template>
  <div class="column">
    <div class="card">
      <header class="card-header">
        <p class="card-header-title has-text-grey">
          {{ title }}
        </p>
      </header>
      <div class="card-content">
        <p>
          <span>
            <slot />
          </span>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ImgCard",
  props: {
    title: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped>
.card {
  height: 255px;
  width: 300px;
}
@media only screen and (max-width: 500px) {
  .card {
    min-height: 300px;
    min-width: 300px;
    justify-content:center;
    align-items:center
  }
}
</style>
