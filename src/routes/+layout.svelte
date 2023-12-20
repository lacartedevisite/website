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
		footer
	</div>
</div>

<script>
    import AppNav from "$lib/AppNav.svelte";
    import "../style/_main.scss"
    import {cardIsOpen} from "../store";
</script>

<style>
	.s-app__nav {
      padding: 1rem;
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      box-sizing: border-box;
      z-index: 1000;
	}
</style>
