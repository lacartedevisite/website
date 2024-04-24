<div
        class="s-app"
>
	<main
          class="s-app__main"
  >
      <img src="/assets/logo.svg"  alt="logo" width="auto" height="50px">
      <p style="font-size: .75rem; line-height: 1.25em; margin-top: 2rem; margin-bottom: 2rem">Se transforme pour devenir</p>
      <p>Atelier Tramons
        <br>Espace associatif dédier à l'imprimerie, Genève
        <br>☆ Impression ☆ Édition ☆ Formation ☆
        <br>Riso 12 couleurs | Press Typo | Offset
      </p>

      <a class="app-button" href="https://tramons.ch/"
         target="_self"
         style="margin-top: 1rem"
      >Accéder au site</a>
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
