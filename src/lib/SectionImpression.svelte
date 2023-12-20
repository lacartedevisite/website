<script>
import Card from "$lib/Card.svelte";
</script>

<section class="s-g-section"
         id="impression"
>
  <div class="s-g-section__title"
  >
    <h2>Impression</h2>
  </div>

  <div class="s-g-section__content"
  >
    <div class="s-g-grid s-g-grid--coll-4"
    >
      <div class="s-g-grid__item"
           style="grid-column: 1 / 3"
      >
        <Card
                styleVariante='is-brown--dark'
        >
          <div slot="recto">
            <h3 class="s-g-font-xxl"
            >Petit format, grande précision: l’art de l’impression miniature
            </h3>
            <div
                    class="s-g-section__card__1__facenord"
            ></div>
          </div>
          <div slot="verso">
            <p>Quand il s’agit d’imprimer des objets de petite taille, chaque millimètre compte. C’est pourquoi nous combinons la précision artisanale avec des technologies contemporaines pour garantir que chaque impression soit une réussite. Notre exigence de qualité signifie que chaque impression, aussi petite soit-elle, est réalisée à la perfection.</p>
            <p>Nous pouvons réaliser :</p>
            <ul>
              <li>Impression Riso A3 jusqu’à 15 couleurs</li>
              <li>Impression sur presse typo</li>
              <li>Gaufrage</li>
              <li>Impression Offset jusqu’au format A4</li>
              <li>Impression à chaud</li>

            </ul>
          </div>
        </Card>
      </div>

      <div
              class="s-g-grid__item"
              style="grid-column: 3 / 5"
      >
        <Card
                styleVariante='is-brown'
        >
          <div slot="recto">
            <h3 class="s-g-font-xl"
            >l’impression en ton direct. disponible en 15 couleurs, 105 combinaisons de bichromie.</h3>
          </div>
          <div slot="verso">

          </div>
        </Card>
      </div>

      <div
              class="s-g-grid__item"
              style="grid-column: 1 / 3"
      >
        <Card
                styleVariante='is-brown'
        >
          <div slot="recto">
            <h3 class="s-g-font-xl"
            >l’impression en ton direct. disponible en 15 couleurs, 105 combinaisons de bichromie.</h3>
          </div>
          <div slot="verso">
            <h2>verso</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae corporis, cumque ducimus eos, est et ex
              excepturi incidunt ipsam itaque non officia perspiciatis porro qui quia quod voluptatem. Eligendi, odit.</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus aspernatur commodi ea eius enim eum
              eveniet inventore iusto magnam nesciunt nisi odit officia quos, repudiandae sunt tempore totam voluptatem
              voluptatum!</p>
          </div>
        </Card>
      </div>



      <div
              class="s-g-grid__item"
              style="grid-column: 3 / 4"
      >
        <Card
                styleVariante='is-brown'
        >
          <div slot="recto">
            <h3 class="s-g-font-xl"
            >l’impression en ton direct. disponible en 15 couleurs, 105 combinaisons de bichromie.</h3>
          </div>
          <div slot="verso">
            <h2>verso</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae corporis, cumque ducimus eos, est et ex
              excepturi incidunt ipsam itaque non officia perspiciatis porro qui quia quod voluptatem. Eligendi, odit.</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus aspernatur commodi ea eius enim eum
              eveniet inventore iusto magnam nesciunt nisi odit officia quos, repudiandae sunt tempore totam voluptatem
              voluptatum!</p>
          </div>
        </Card>
      </div>



      <div
              class="s-g-grid__item"
              style="grid-column: 4 / 5"
      >
        <Card
                styleVariante='is-brown'
        >
          <div slot="recto">
            <h3 class="s-g-font-xl"
            >l’impression en ton direct. disponible en 15 couleurs, 105 combinaisons de bichromie.</h3>
          </div>
          <div slot="verso">
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

<style lang="scss" >
.s-g-section__card__1__facenord {
  position: relative;
  width: 100%;
  padding-top: 100%;
  background: red;
}
</style>
