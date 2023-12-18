<div
        class="s-card s-g-background-linear-v1"
        class:is-open={isOpen}
>
  <button
          on:click={toggleCardPosition}
          class="s-g-ui--button-rounded s-card__button"
  >

  </button>

  <div
          class="s-card__content"
  >
    <slot name="recto"/>
    <slot name="verso" />
  </div>
</div>

<script lang="ts" >
    let isOpen = false

    function toggleCardPosition() {
        isOpen = !isOpen
    }
</script>

<style lang="scss" >
  .s-card {
    position: relative;
    padding:        var(--s-radius);
    border-radius:  var(--s-radius);


  }

  .s-card__button {
    position: absolute;
    bottom: .5rem;
    right: .5rem;
  }

  .s-card__content {
    &.is-open {

    }
  }

</style>
