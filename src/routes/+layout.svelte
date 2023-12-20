<div
        class="s-app"
        class:card-is-open={$cardIsOpen}
>
	<div
					class="s-app__nav"
	>
    <AppNav/>
	</div>

  <div>

  </div>

	<main
          class="s-app__main"
  >
		<slot />
	</main>

	<div
          class="s-app__footer"
  >
		<div>
      <button on:click={() => {window.scrollTo({top: 0, behavior: "smooth"})}}
      >
        <img alt="logo"
             src="/assets/logo-black.svg"
             class="s-app__nav__logo"
        >
      </button>
    </div>
    <div>
      RUE MARGUERITE DELLENBACH 5
      <br>1205 GENÈVE
    </div>
	</div>
</div>

<script>
    import AppNav from "$lib/AppNav.svelte";
    import "../style/_main.scss"
    import {cardIsOpen} from "../store";
</script>

<style lang="scss">
  .s-app__nav {
    padding: 1rem;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    box-sizing: border-box;
    z-index: 1000;
  }

  .s-app__footer {
    display: flex;
    align-items: center;
    justify-content: space-between;
    border-top: solid 1px black;
    padding-top: 1rem;

    button {
      all: unset;
      cursor: pointer;
      user-select: none;
    }
  }

  .s-app__nav__logo {
    display: block;
    height: 2rem;
    width: auto;
  }
</style>
