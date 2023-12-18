<div class="s-app">
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
</script>

<style>
	.app {
	}

	main {
	}
</style>
