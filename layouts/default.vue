<template>
  <div>
    <nav
      class="navbar header has-shadow is-primary"
      id="big"
      role="navigation"
      aria-label="main navigation"
    >
      <div class="navbar-brand">
        <a
          class="navbar-item"
          href="/"
        >
          <img
            src="~assets/sepulcher.png"
            alt="Buefy"
            height="28"
          >
        </a>
      </div>
    </nav>

    <section class="main-content columns">
      <aside class="column is-2 section">
        <p class="menu-label is-hidden-touch">
          Menu
        </p>
        <ul class="menu-list">
          <li
            v-for="(item, key) of items"
            :key="key"
          >
            <NuxtLink
              :to="item.to"
              exact-active-class="is-active"
            >
              <b-icon :icon="item.icon" /> {{ item.title }}
            </NuxtLink>
          </li>
        </ul>
      </aside>

      <div class="container column is-10">
        <Nuxt />
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data () {
    return {
      items: [
        {
          title: 'My work',
          icon: 'briefcase',
          to: { name: 'index' }
        },
        {
          title: 'About me',
          icon: 'alien',
          to: { name: 'about' }
        },
        {
          title: 'Contact',
          icon: 'cellphone',
          to: { name: 'contact' }
        }
      ]
    }
  }
}
</script>

<style scoped>
#big{
  min-height: 150px;
  display:flex;
  align-items: center
}

img{
  filter: invert(100%);
}
</style>
