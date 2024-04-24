<div
        class="s-app"
>
	<main
          class="s-app__main"
  >
    <slot/>
    </main>
</div>

<script lang="ts">
    import "../style/_main.scss"
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
  }

  .s-app__main {
    box-sizing: border-box;
    padding: 2rem;
    width: 100%;
  }


</style>
