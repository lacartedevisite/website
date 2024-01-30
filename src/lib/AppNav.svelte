<nav
        class="s-app-nav"
>
  <button on:click={() => document.querySelector('.s-app')?.scrollTo({top: 0, behavior: "smooth"})}
  >
    <img class="s-app-nav__logo"
         alt="logo"
         src="/assets/logo.svg"
    >
  </button>

  <a class="s-app-nav__text-link s-remove-mobile-on-version" href="#impression"   >IMPRESSION</a>
  <a class="s-app-nav__text-link s-remove-mobile-on-version" href="#graphisme"    >GRAPHISME</a>
  <a class="s-app-nav__text-link s-remove-mobile-on-version" href="#reproduction" >REPRODUCTION</a>
  <a class="s-app-nav__text-link s-remove-mobile-on-version" href="#about"       >À PROPOS</a>

  <a
          href="mailto:clovis@lacartevisite.ch"
          target="_blank"
  >
    <img  class="s-app-nav__mailto-icon"
          alt="mailto"
          src="/assets/icon-mail-open.svg"
    />
  </a>

</nav>

<script lang="ts">
</script>

<style lang="scss">
.s-app-nav {
  display: flex;
  justify-content: space-between;
  background: var(--s-color--purple--opcaity-60);
  color: white;
  height: var(--s-nav-height);
  align-items: center;
  border-radius: 3rem;
  padding-left: 1rem;
  padding-right: 1rem;
  backdrop-filter: blur(8px);
  -webkit-backdrop-filter: blur(8px);
}

a {
  display: block;
  color: inherit;
  text-decoration: none;
}

.s-app-nav__text-link {
  padding-top: .25em;
}

button {
  all: unset;
  cursor: pointer;
  user-select: none;
}

img {
  display: block;
}

.s-app-nav__logo {
  display: block;
  height: calc( var(--s-nav-height) - .80rem);
}

.s-app-nav__mailto-icon {
  display: block;
  height: calc( var(--s-nav-height) - 1.5rem);
  position: relative;
}

</style>
