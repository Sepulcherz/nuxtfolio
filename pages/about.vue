<template>
  <section>
    <h1 class="aboutstyle title is-3 has-text-grey">
      Hello. I'm Matthias, A junior web developper from France. <br>
      I'm also known as Sepulcher or SepulcherZ
    </h1>
    <p class="aboutstyle title is-6">
      I recently learned how to code a few months ago (and still learning) and I decided to
      create this portfolio so you can see what I accomplished so far.
    </p>
    <br />
    <p class="aboutstyle2 title is-6">
      Since I was little, I had a great interest in computers and art.
    </p>
    <p class="aboutstyle2 title is-6">
      Which is why I got my hands on 3D and web developpement.
    </p>
    <p class="aboutstyle2 title is-6">
      I also try to make music when I feel like it, but nothing really serious.
    </p>
    <br />
    <p class="aboutstyle2 title is-6">
      Oh, and I also stream every now and then, feel free to come by! 
    </p>
    <p class="aboutstyle2 title is-6">
      <a>https://www.twitch.tv/sepulcherz</a>
    </p>
  </section>
</template>

<script>
import Card from "~/components/Card";

export default {
  name: "AboutPage",
  components: {
    Card,
  },
};
</script>

<style>
.aboutstyle {
  margin-top: 5rem;
}
.aboutstyle2 {
  margin-top: 1rem;
}

@media only screen and (max-width: 500px){
  h1{
    margin:0.5em
  }
  p{
    margin:1em
  }
}
</style>
