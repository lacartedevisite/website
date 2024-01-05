<script>
    import Card from "$lib/Card.svelte";
</script>

<section
        class="s-g-section"
        id="graphisme"
>
  <div class="s-g-section__title"
  >
    <h2>Graphisme</h2>
  </div>
  <div
          class="s-g-section__content"
  >
    <div class="s-g-grid s-g-grid--coll-4"
    >
      <div class="s-g-grid__item"
           style="grid-column: 1 / 5"
      >
        <Card
                styleVariante='is-yellow'
                title="GRAPHISME"
        >
          <div slot="recto">
            <div class="s-g-section__card__graphisme s-g-remove-child-margin">
              <h3 class="s-g-font-l s-g-section__card__graphisme__title"
              >L’ACCOMPAGNEMENT SUR-MESURE POUR VOS PROJETS CRÉATIFS</h3>
              <div class="s-g-section__card__graphisme__img-box"
              ></div>
            </div>
          </div>
          <div slot="verso" class="s-g-remove-child-margin">
            <h2>verso</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae corporis, cumque ducimus eos, est et ex
              excepturi incidunt ipsam itaque non officia perspiciatis porro qui quia quod voluptatem. Eligendi, odit.</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus aspernatur commodi ea eius enim eum
              eveniet inventore iusto magnam nesciunt nisi odit officia quos, repudiandae sunt tempore totam voluptatem
              voluptatum!</p>
          </div>
        </Card>
      </div>
    </div>
  </div>
</section>

<style lang="scss">
  .s-g-section__card__graphisme {
    display: flex;
    flex-direction: row;
    padding: 1rem;
    gap: 1rem;
    flex-wrap: nowrap;
  }

  .s-g-section__card__graphisme__title {
    width: 50%;
    text-align: center;
  }
  .s-g-section__card__graphisme__img-box {
    width: 50%;
    background: red;
    padding-top: 50%;
  }
</style>
