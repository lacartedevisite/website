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
                titleColor="#646464"
                backgroundFrontCard="transparent conic-gradient(from 90deg at 50% 103%, #BBAF86 0.00%, #FFD490 100.00%) 0% 0% no-repeat padding-box"
        >
          <div slot="recto">
            <div class="s-g-section__card__graphisme s-g-remove-child-margin">
              <h3 class="s-g-font-l s-g-section__card__graphisme__title"
              >L’ACCOMPAGNEMENT SUR-MESURE POUR VOS PROJETS CRÉATIFS</h3>
              <div class="s-g-section__card__graphisme__img-box"
              >
                <img src="/assets/imgs/graphisme.jpg"
                     alt="image graphisme"
                />
              </div>
            </div>
          </div>
          <div slot="verso" class="s-g-remove-child-margin">
            <p>A la Carte de Visite, nous vous aidons pour le développement de vos projets graphiques selon vos besoins : conception graphique, conseil, accompagnement de projet ou exécution.</p>
            <p>Dans le domaine du graphisme, "La Carte de Visite" se distingue par son expertise et son approche personnalisée. Nous vous accompagnons dans vos projets créatifs, avec une attention particulière portée à la micro édition.</p>
            <p>Notre service de graphisme s'étend de la conception initiale à la réalisation finale, assurant que chaque aspect de votre projet reflète votre vision. Que vous cherchiez à créer des brochures, des livres d'art, des magazines ou tout autre support imprimé, nous garantissons une réalisation soignée et une attention aux détails.</p>
            <h3>Un Service complet</h3>
            <p>De la conception graphique au choix des matériaux, en passant par la mise en page et l'impression, nous offrons un service complet. Notre engagement envers la qualité se manifeste dans chaque étape du processus.</p>

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
    align-items: center;

    @media (max-width: 860px) {
      flex-direction: column-reverse;
    }
  }

  .s-g-section__card__graphisme__title {
    width: 50%;
    text-align: center;

    @media (max-width: 860px) {
      width: 100%;
    }
  }
  .s-g-section__card__graphisme__img-box {
    width: 50%;

    @media (max-width: 860px) {
      width: 100%;
    }

    > img {
      display: block;
      width: 100%;
      height: auto;
    }
  }
</style>
