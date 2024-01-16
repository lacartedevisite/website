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
      <button
              on:click={closeCards}
              in:scaleRotate
              out:scaleRotate
              class="s-g-ui--button-rounded s-card__button s-app__button-close"
              style="background-color: white"
      >
        <UIButtonAdd isBlack="{true}"/>
      </button>
    {/if}
  </main>


	<div
          class="s-app__footer"
  >
    <div class="s-app__footer__box"
    >
      <div class="s-app__footer__box__line"></div>
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

<script lang="ts">
    import AppNav from "$lib/AppNav.svelte";
    import "../style/_main.scss"
    import {cardIsOpen} from "../store";
    import {fade} from "svelte/transition"
    import UIButtonAdd from "$lib/UIButtonAdd.svelte";


    function closeCards() {
        cardIsOpen.update(value => false)
    }

    // animation fun
    function scaleRotate(el: Node, params: any, options: { direction: 'in' | 'out' | 'both' }): {
      duration?: number,
      delay?: number,
      easing?: (t: number) => number,
      css?: (t: number, u: number) => string,
      tick?: (t: number, u: number) => void
    } {

      return {
        delay: options.direction === 'in' ? 1000 : 0,
        duration: 500,
        easing: t => t * t * t,
        css: (t, u) => `transform: scale(${t}) rotate(${t * 90}deg)`
      }
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
    scrollbar-gutter: stable;

    &.card-is-open {
      overflow: hidden;
    }
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
      padding: 1rem;
      box-sizing: border-box;
      max-width: var(--s-site-max-width);
      flex-wrap: wrap;
      margin: 1rem auto auto;
      position: relative;
      gap: 1rem;
    }
  }

  .s-app__footer__box__line {
    width: calc( 100% - 2rem );
    height: 1px;
    background: black;
    position: absolute;
    top: 0;
    left: 1rem;
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

  .s-app__button-close {
    position: fixed;
    bottom: 1rem;
    right: 1rem;
    z-index: 99999999999999999999;

    :global(> *) {
      transform: rotate(45deg);
    }
  }
</style>
