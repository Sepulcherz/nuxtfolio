<template>
  <div>
    <section class="section">
      <h1 class="aboutstyle2 title is-3 has-text-grey">Web</h1>
      <div class="columns is-mobile">
        <div class="cardz">
          <imgCard title="My 'crazy' resume">
            <a href="https://sepulcherz.github.io/CV/" target="blank"
              ><img src="~assets/cv.png" alt="Sepulcher"
            /></a>
          </imgCard>
        </div>

        <div class="cardz">
          <imgCard title="Playing around with AnimeJS">
            <a
              href="https://github.com/Sepulcherz/AnimeJsTry---Blocks"
              target="blank"
              ><img src="~assets/blocks.png" alt="Sepulcher"
            /></a>
          </imgCard>
        </div>

        <div class="cardz">
          <imgCard title="My first React static app">
            <a href="https://github.com/Sepulcherz/reac-test" target="blank"
              ><img src="~assets/react.png" alt="Sepulcher"
            /></a>
          </imgCard>
        </div>
      </div>
    </section>

    <section class="section">
      <h1 class="aboutstyle2 title is-3 has-text-grey">Original Creations</h1>
      <div class="columns is-mobile">
        <div class="cardz">
          <imgCard title="Autoportrait">
            <a href="https://www.instagram.com/p/CPidbmYgotA/" target="blank"
              ><img src="~assets/sepulcherzzz.png" alt="Sepulcher"
            /></a>
          </imgCard>
        </div>

        <div class="cardz">
          <imgCard title="Something weird">
            <a href="https://www.instagram.com/p/CPieIrTA3gV/" target="blank"
              ><img src="~assets/whatever.png" alt="Sepulcher"
            /></a>
          </imgCard>
        </div>

        <div class="cardz">
          <imgCard title="An eye, kinda">
            <a href="https://www.instagram.com/p/CPid99_g1Wy/" target="blank"
              ><img src="~assets/eyez.png" alt="Sepulcher"
            /></a>
          </imgCard>
        </div>
      </div>
    </section>
    <section class="section">
      <div class="columns is-mobile">
        <div class="cardz">
          <imgCard title="My first Sculpt on blender">
            <a href="https://www.instagram.com/p/CPid4-CAlRy/" target="blank"
              ><img src="~assets/boulbabiert.png" alt="Sepulcher"
            /></a>
          </imgCard>
        </div>

        <div class="cardz">
          <imgCard title="Sachiel but this is my head">
            <a href="https://www.instagram.com/p/CPifAoRAnIF/" target="blank"
              ><img src="~assets/sachielthiass.png" alt="Sepulcher"
            /></a>
          </imgCard>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import Card from "~/components/Card";

export default {
  name: "MyWorkPage",
};
</script>

<style scoped>
@media only screen and (max-width: 500px) {
  .columns .is-mobile {
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .cardz {
    margin-bottom: 5em;
  }
}
img {
  border-radius: 5px;
  object-fit: cover;
  min-height: 150px;
  max-height: 150px;
  min-width: 220px;
}
.cardz {
  height: 255px;
  width: 300px;
}
.section {
  margin-top: -3em;
}
</style>
