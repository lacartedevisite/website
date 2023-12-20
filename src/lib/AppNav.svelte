<nav
        class="s-app-nav "
>
  <button on:click={() => {window.scrollTo({top: 0, behavior: "smooth"})}}
  >
    <img alt="logo"
         src="/assets/logo.svg"
    >
  </button>

  <a href="#impression"   >IMPRESSION</a>
  <a href="#graphisme"    >GRAPHISME</a>
  <a href="#reproduction" >REPRODUCTION</a>
  <a href="#about"       >À PROPOS</a>

  <a
          href="mailto:hello@lacartedevisite.ch"
          target="_blank"
  >
    <img
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
  height: 3rem;
  align-items: center;
  border-radius: 3rem;
  padding-left: 1rem;
  padding-right: 1rem;
  backdrop-filter: blur(8px);
  -webkit-backdrop-filter: blur(8px);
}

a {
  color: inherit;
  text-decoration: none;
}

button {
  all: unset;
  cursor: pointer;
  user-select: none;
}

img {
  display: block;
}

</style>
