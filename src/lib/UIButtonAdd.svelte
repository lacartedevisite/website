<svg    class="s-ui-button-add"
        class:is-black={isBlack}
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 -960 960 960"
><path d="M440-440H200v-80h240v-240h80v240h240v80H520v240h-80v-240Z"/></svg>

<script>
  export let isBlack = false
</script>

<style lang="scss">
  .s-ui-button-add {
    fill: white;
    display: block;

    &.is-black {
      * {
        fill: black;
      }
    }
  }

</style>
