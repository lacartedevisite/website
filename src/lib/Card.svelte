<div
        class="s-card {styleVariante}"
        class:is-open={isOpen}
>
  <button
          on:click={toggleCardPosition}
          class="s-g-ui--button-rounded s-card__button"
          style="background-color: {buttonColor}"
  >
    <UIButtonAdd isBlack="{buttonIconIsBlack}" />
  </button>

  <div class="s-card__content"
       bind:this={cardContent}
  >
    <div class="s-card__content__face s-card__content__face--front"
         class:s-g-background-linear-brown--dark    ={styleVariante === 'is-brown--dark'}
         class:s-g-background-linear-brown          ={styleVariante === 'is-brown'}
         class:s-g-background-linear-brown--light   ={styleVariante === 'is-brown--light'}
         class:s-g-background-linear-green          ={styleVariante === 'is-green'}
         class:s-g-background-linear-grey           ={styleVariante === 'is-grey'}
         class:s-g-background-linear-yellow         ={styleVariante === 'is-yellow'}
         class:s-g-background-linear-purple         ={styleVariante === 'is-purple-gradient'}
    >
      {#if title}
        <h3 class="s-card__title">{title}</h3>
      {/if}
      <slot name="recto"/>
    </div>
    <div class="s-card__content__face s-card__content__face--back"
    >
      <slot name="verso"/>
    </div>
  </div>
</div>

<script lang="ts" >
    import {cardIsOpen} from "../store";
    import UIButtonAdd from "$lib/UIButtonAdd.svelte";

    let isOpen = false
    let cardContent: HTMLDivElement | undefined

    export let styleVariante: 'is-brown--dark' | 'is-brown' | 'is-brown--light' | 'is-purple' | 'is-green' | 'is-grey' | 'is-yellow' | 'is-purple-gradient'
    export let title: string | null = null
    export let buttonIconIsBlack = false
    export let buttonColor = '#000'

    function toggleCardPosition() {
        isOpen = !isOpen
        cardIsOpen.update(value => isOpen)
        updateCardTransformation()
    }

    cardIsOpen.subscribe(value => {
        if (!value) {
            isOpen = false
            updateCardTransformation()
        }
    })

    function updateCardTransformation() {
        if(cardContent) {
            const cardRect = cardContent.getBoundingClientRect()

            const centerX = cardRect.left + cardRect.width / 2
            const centerY = cardRect.top + cardRect.height / 2

            const screenCenterX = window.innerWidth / 2
            const screenCenterY = window.innerHeight / 2

            if(isOpen) cardContent.style.transform = `rotate3d(0, 1, 0, 180deg) translate(${centerX - screenCenterX}px, ${screenCenterY - centerY}px)`
            else cardContent.style.transform = 'none'
        }

    }
</script>

<style lang="scss" >
  .s-card {
    position: relative;
    perspective: 2000px;
    display: flex;
    z-index: 1;
    transition: z-index 0s .5s;
    width: 100%;

    &.is-open {
      z-index: 1000000;
    }
  }

  .s-card__button {
    position: absolute;
    bottom: .5rem;
    right: .5rem;
    z-index: 1000;
    display: flex;
    align-items: center;
    justify-content: center;


    :global(> *) {
      width: 1.5rem;
    }
  }

  .s-card__content {
    transform: rotate3d(0, 0, 0, 0deg);
    transform-origin: center center;
    transition: transform 1s ease-in-out;
    transform-style: preserve-3d;
    position: relative;
    display: flex;
    width: 100%;

    .is-open & {
      transform:
              rotate3d(0, 1, 0, 180deg)
              translate(250px, 70px);
    }
  }

  .s-card__title {
    padding: 1rem;
    margin: 0;
    position: relative;
    z-index: 10;
  }

  .s-card__content__face {
    box-sizing: border-box;
    -webkit-backface-visibility: hidden; /* Safari */
    backface-visibility: hidden;
    border-radius:  var(--s-radius);
    width: 100%;
    overflow: hidden;
  }

  .s-card__content__face--front {
    position: relative;

    .is-purple & {
      background: var(--s-color--purple-light);
    }

    .is-yellow & {
      background: var(--s-color--yellow);
    }
  }

  .s-card__content__face--back {
    transform: translate(-50%, -50%) rotateY(180deg);
    position: absolute;
    width: 100%;
    height: 100%;
    top: 50%;
    left: 50%;
    max-width: 40rem;
    transition: width 1s ease-in-out, height 1s ease-in-out;
    background-color: white;
    padding: 1rem;
    border: solid 10px var(--s-color--brown-yellow--light);

    .is-open & {
      width:  calc(100vw - 2rem);
      height: calc(100vh - 6rem);
    }
  }

  :global([slot="recto"]) {
    :global(> *:first-child) {
      margin-top: 0;
    }
    :global(> *:last-child) {
      margin-bottom: 0;
    }
  }

  .is-brown--dark {
    :global(h3) {
      color: var(--s-color--brown-yellow--light);
    }
  }

  .is-brown {
    :global(h3) {
      color: var(--s-color--brown-yellow--light);
    }

    .s-card__title {
      color: var(--s-color--grey--dark);
    }
  }

  .is-brown--light {
    :global(h3) {
      color: var(--s-color--brown);
    }
  }

  .is-green {
    :global(*) {
      color: var(--s-color--purple-light);
    }
  }

  .is-purple {
    :global(*) {
      color: white;
    }
  }

  .is-grey,
  .is-purple-gradient {
    :global(*) {
      color: var(--s-color--brown--light);
    }
  }

  button {
    position: relative;
    z-index: 10;
  }
</style>

