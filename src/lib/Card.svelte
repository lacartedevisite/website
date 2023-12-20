<div
        class="s-card {styleVariante}"
        class:is-open={isOpen}
>
  <button
          on:click={toggleCardPosition}
          class="s-g-ui--button-rounded s-card__button"
  >

  </button>

  <div class="s-card__content"
  >
    <div class="s-card__content__face s-card__content__face--front"
         class:s-g-background-linear-brown--dark  ={styleVariante === 'is-brown--dark'}
         class:s-g-background-linear-brown        ={styleVariante === 'is-brown'}
         class:s-g-background-linear-brown--light ={styleVariante === 'is-brown--light'}
    >
      <slot name="recto"/>
    </div>
    <div class="s-card__content__face s-card__content__face--back s-g-background-linear-brown"
    >
      <slot name="verso"/>
    </div>
  </div>
</div>

<script lang="ts" >
    import {cardIsOpen} from "../store";

    let isOpen = false

    export let styleVariante: 'is-brown--dark' | 'is-brown' | 'is-brown--light'

    function toggleCardPosition() {
        cardIsOpen.update(value => !value)
        isOpen = !isOpen
    }
</script>

<style lang="scss" >
  .s-card {
    position: relative;
    perspective: 2000px;
    display: flex;
    z-index: 1;
    transition: z-index 0s .5s;

    &.is-open {
      z-index: 1000000;
    }
  }

  .s-card__button {
    position: absolute;
    bottom: .5rem;
    right: .5rem;
    z-index: 1000;
  }

  .s-card__content {
    transform: rotate3d(0, 0, 0, 0deg);
    transition: transform 1s ease-in-out;
    transform-style: preserve-3d;
    position: relative;

    .is-open & {
      transform:
              //rotate3d(1, 0, 0, 180deg)
              rotate3d(0, 1, 0, 180deg)
              //rotate3d(0, 0, 1, 180deg)
              translate(250px, 70px);
    }
  }

  .s-card__content__face {
    box-sizing: border-box;
    -webkit-backface-visibility: hidden; /* Safari */
    backface-visibility: hidden;
    padding:        var(--s-radius);
    border-radius:  var(--s-radius);
    min-height: 100%;
  }

  .s-card__content__face--front {
    position: relative;
  }

  .s-card__content__face--back {
    transform: rotateY(180deg);
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    max-width: 40rem;
    transition: width 1s ease-in-out, height 1s ease-in-out;

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
      color: var(--s-color--brown--yellow);
    }
  }

  .is-brown {
    :global(h3) {
      color: var(--s-color--brown--yellow);
    }
  }

  .is-brown--light {
    :global(h3) {
      color: var(--s-color--brown);
    }
  }
</style>

