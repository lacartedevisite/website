<header class="s-section-intro"
>
  <div class="s-section-intro__box s-g-background-linear-purple--light"
  >
    <h2 class="s-g-font-xl s-section-intro__title"
    >impression typo
      <br/>risographie
      <br/>OFFSET
      <br/>
      <br/>la carte de visite est un lieu associatif spécialisé dans le&nbsp;petit&nbsp;format.
      <img alt="icon hirondelle.svg"  src="/assets/hirondelle.svg" class="s-section-intro__title__hirondelle s-section-intro__title__hirondelle--top-left" />
      <img alt="icon hirondelle.svg"  src="/assets/hirondelle.svg" class="s-section-intro__title__hirondelle s-section-intro__title__hirondelle--top-right" />
      <img alt="icon hirondelle.svg"  src="/assets/hirondelle.svg" class="s-section-intro__title__hirondelle s-section-intro__title__hirondelle--bottom-right" />
      <img alt="icon hirondelle.svg"  src="/assets/hirondelle.svg" class="s-section-intro__title__hirondelle s-section-intro__title__hirondelle--bottom-left" />
      <img alt="icon mire.svg"        src="/assets/mire.svg"       class="s-section-intro__title__mire s-section-intro__title__hirondelle--left"/>
      <img alt="icon mire.svg"        src="/assets/mire.svg"       class="s-section-intro__title__mire s-section-intro__title__hirondelle--right"/>
    </h2>
  </div>
</header>

<style lang="scss">

  .s-section-intro {
    display: flex;
    align-items: center;
    justify-content: center;
    box-sizing: border-box;
    width: 100%;
    padding: calc( var(--s-nav-height) + 2rem) 0 0 0;
  }

  .s-section-intro__box {
    //min-height: calc(100vh - var(--s-nav-height) - 7rem);
    width: 100%;
    position: relative;
    border-radius: var(--s-radius);
    display: flex;
    align-items: center;
    padding: 10rem 2rem;
  }

  .s-section-intro__title {
    padding: 2rem 4rem;
    position: relative;
    margin: auto;
  }

  .s-section-intro__title__hirondelle{
    position: absolute;
  }

  .s-section-intro__title__hirondelle--top-left {
    top: 0;
    left: 0;
  }

  .s-section-intro__title__hirondelle--top-right {
    top: 0;
    right: 0;
    transform: rotate(90deg);
  }

  .s-section-intro__title__hirondelle--bottom-right {
    bottom: 0;
    right: 0;
    transform: rotate(180deg);
  }

  .s-section-intro__title__hirondelle--bottom-left {
    bottom: 0;
    left: 0;
    transform: rotate(270deg);
  }

  .s-section-intro__title__mire {
    position: absolute;
    transform: translate(0, -50%);
  }
  .s-section-intro__title__hirondelle--left {
    top: 50%;
    left: 0;
  }

  .s-section-intro__title__hirondelle--right {
    top: 50%;
    right: 0;
  }
</style>
