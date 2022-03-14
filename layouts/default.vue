<template>
  <div>
    <nav
      class="navbar header has-shadow is-primary"
      id="big"
      role="navigation"
      aria-label="main navigation"
    >
      <div class="navbar-brand">
        <a class="navbar-item" href="/">
          <img src="~assets/sepulcher.png" alt="Sepulcher_logo" height="28" />
        </a>
      </div>
      <div class="marginleft">
        <div class="navbar-brand">
          <a
            class="navbar-item"
            href="https://github.com/Sepulcherz"
            target="_blank"
          >
            <b-icon icon="github" />
          </a>
        </div>

        <div class="navbar-brand">
          <a
            class="navbar-item"
            href="https://www.linkedin.com/in/matthias-devaux-768740188/"
            target="_blank"
          >
            <b-icon icon="linkedin" />
          </a>
        </div>
      </div>
    </nav>
    <section class="main-content columns">
      <aside class="column is-2 section">
        <p class="menu-label is-hidden-touch">Menu</p>
        <ul class="menu-list">
          <li v-for="(item, key) of items" :key="key">
            <NuxtLink :to="item.to" exact-active-class="is-active">
              <b-icon :icon="item.icon" /> {{ item.title }}
            </NuxtLink>
          </li>
        </ul>
      </aside>

      <div class="container column is-10">
        <Nuxt />
      </div>
    </section>
    <footer class="footerz title is-6">© Matthias Devaux 2022</footer>
  </div>
</template>

<script>
export default {
  name: "DefaultLayout",
  data() {
    return {
      items: [
        {
          title: "About me",
          icon: "alien",
          to: { name: "index" },
        },
        {
          title: "My work",
          icon: "briefcase",
          to: { name: "my_work" },
        },
        {
          title: "Contact",
          icon: "cellphone",
          to: { name: "contact" },
        },
      ],
    };
  },
};
</script>

<style scoped>
#big {
  min-height: 150px;
  display: flex;
  align-items: center;
}

img {
  filter: invert(100%);
  min-height: 35px;
}

.marginleft {
  margin-left: auto;
  margin-right: 1.5em;
  display: flex;
  width: 100%;
  justify-content: flex-end;
}

</style>
