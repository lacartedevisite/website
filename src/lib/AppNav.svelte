<nav
        class="s-app-nav "
>
  <button
          on:click={() => {window.scrollTo({top: 0, behavior: "smooth"})}}
  >logo</button>

  <a href="#impression"   >IMPRESSION</a>
  <a href="#graphisme"    >GRAPHISME</a>
  <a href="#reproduction" >REPRODUCTION</a>
  <a href="#propos"       >À PROPOS</a>

  <div>mail icon</div>

</nav>

<script lang="ts">
</script>

<style lang="scss">
.s-app-nav {
  display: flex;
  justify-content: space-around;
  background: var(--s-color--purple--opcaity-60);
  color: white;
  height: 3rem;
  align-items: center;
  border-radius: 3rem;
}


</style>
