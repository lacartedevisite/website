<div
        class="s-app"
        class:card-is-open={$cardIsOpen}
>
	<div class="s-app__nav"
	>
    <div class="s-app__nav__max-width"
    >
      <AppNav/>
    </div>
	</div>

	<main
          class="s-app__main"
  >
    <slot/>
    {#if $cardIsOpen}
      <div class="s-app__nav__cache"
           transition:fade={{ delay: 500, duration: 500}}
           on:click={closeCards}
      ></div>
    {/if}
  </main>


	<div
          class="s-app__footer"
  >
    <div class="s-app__footer__box"
    >
      <div style="width: 100%; height: 1px; background: black"></div>
      <div>
        <button on:click={() => document.querySelector('.s-app')?.scrollTo({top: 0, behavior: "smooth"})}
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
</div>

<script>
    import AppNav from "$lib/AppNav.svelte";
    import "../style/_main.scss"
    import {cardIsOpen} from "../store";
    import {fade} from "svelte/transition"


    function closeCards() {
        cardIsOpen.update(value => {return false})
    }
</script>

<style lang="scss">
  .s-app {
    scroll-behavior: smooth;
    -webkit-overflow-scrolling: touch;
    position: relative;
    width: 100%;
    height: 100%;
    overflow: auto;
    box-sizing: border-box;
  }

  .s-app__nav {
    padding: 1rem;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    box-sizing: border-box;
    z-index: 1000;

    .s-app__nav__max-width {
      max-width: var(--s-site-max-width);
      margin: auto;
    }
  }

  .s-app__main {
    box-sizing: border-box;
    padding-left: 1rem;
    padding-right: 1rem;
    max-width: var(--s-site-max-width);
    margin: auto;
  }

  .s-app__footer {
    box-sizing: border-box;
    width: 100%;
    padding-left: 1rem;
    padding-right: 1rem;
    margin-top: 2rem;
    padding-bottom: 1rem;

    button {
      all: unset;
      cursor: pointer;
      user-select: none;
    }

    .s-app__footer__box {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0 1rem;
      box-sizing: border-box;
      max-width: var(--s-site-max-width);
      margin: auto;
      flex-wrap: wrap;
    }
  }


  .s-app__nav__logo {
    display: block;
    height: 2rem;
    width: auto;
  }

  .s-app__nav__cache {
    background: rgba(0, 0, 0, 0.5);
    backdrop-filter: blur(8px);
    -webkit-backdrop-filter: blur(8px);
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: 1;
  }
</style>
