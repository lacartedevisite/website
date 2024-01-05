<script>
import Card from "$lib/Card.svelte";
import UIButtonAdd from "$lib/UIButtonAdd.svelte";
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
                buttonIconIsBlack="{true}"
                buttonColor="white"
        >
          <div slot="recto">
            <div class="s-g-section__card__1__facenord s-g-remove-child-margin"
            >
              <h3 class="s-g-font-xxl s-g-section__card__1__facenord__title"
                >Petit format, grande précision: l’art de l’impression miniature
              </h3>
              <div class="s-g-section__card__1__facenord__img-box"
              >
                <img alt="" src="/assets/imgs/carte_facenord_verso.jpg"/>
              </div>
            </div>
          </div>
          <div slot="verso" class="s-g-remove-child-margin">
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
                title="RISOGRAPHIE"
                buttonIconIsBlack="{false}"
                buttonColor="black"
        >
          <div slot="recto">
            <div class="s-g-section__card__2__riso s-g-remove-child-margin">
              <h3 class="s-g-font-xl"
              >l’impression en ton direct. disponible en 15 couleurs, 105 combinaisons de bichromie.
              </h3>
              <div class="s-g-section__card__2__riso__options-box"
              >
                <div class="s-g-ui-option s-g-ui-option--flat-gold"           >Flat Gold</div>
                <div class="s-g-ui-option s-g-ui-option--black-hd"            >Black HD</div>
                <div class="s-g-ui-option s-g-ui-option--medium-blue"         >Medium Blue</div>
                <div class="s-g-ui-option s-g-ui-option--metallic-silver"     >Metallic Silver</div>
                <div class="s-g-ui-option s-g-ui-option--fluorescent-yellow"  >Fluorescent Yellow</div>
                <div class="s-g-ui-option s-g-ui-option--brown"               >Brown</div>
                <div class="s-g-ui-option s-g-ui-option--green"               >Green</div>
                <div class="s-g-ui-option s-g-ui-option--fluorescent-red"     >Fluorescent red</div>
                <div class="s-g-ui-option s-g-ui-option--orange"              >Orange</div>
                <div class="s-g-ui-option s-g-ui-option--fluorescent-green"   >Fluorescent green</div>
                <div class="s-g-ui-option s-g-ui-option--purple"              >Purple</div>
                <div class="s-g-ui-option s-g-ui-option--metallic-gold"       >Mettalic Gold</div>
                <div class="s-g-ui-option s-g-ui-option--blue"                >Blue</div>
                <div class="s-g-ui-option s-g-ui-option--yellow"              >Yellow</div>
                <div class="s-g-ui-option s-g-ui-option--bright-red"          >Bright Red</div>
              </div>
            </div>
          </div>
          <div slot="verso" class="s-g-remove-child-margin">

          </div>
        </Card>
      </div>

      <div
              class="s-g-grid__item"
              style="grid-column: 1 / 3"
      >
        <Card
                styleVariante='is-brown'
                title="TYPO"
        >
          <div slot="recto">
            <div class="s-g-section__card__3__heidelberg s-g-remove-child-margin">
              <h3 class="s-g-font-l s-g-section__card__3__heidelberg__title"
              >L’original Heidelberg Pour vos compositions typographiques</h3>
              <div class="s-g-section__card__3__heidelberg__img-box"
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



      <div
              class="s-g-grid__item"
              style="grid-column: 3 / 4"
      >
        <Card
                styleVariante='is-brown'
                title="GAUFRAGE"
        >
          <div slot="recto">
            <div class="s-g-section__card__4 s-g-remove-child-margin"
            >
              <h3 class="s-g-font-l s-g-section__card__4__title"
              >Du volume dans vos imprimés</h3>
              <div class="s-g-section__card__4__img-box"
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



      <div
              class="s-g-grid__item"
              style="grid-column: 4 / 5"
      >
        <Card
                styleVariante='is-brown'
                title="OFFSET"
        >
          <div slot="recto">
            <div class="s-g-section__card__5 s-g-remove-child-margin"
            >
              <h3 class="s-g-font-l s-g-section__card__5__title"
              >L’impression offset une couleur format A4</h3>
              <div class="s-g-section__card__5__img-box"
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

      <div
              class="s-g-grid__item"
              style="grid-column: 1 / 5"
      >
        <Card
                styleVariante='is-brown'
                title="Folio"
        >
          <div slot="recto">
            <div class="s-g-section__card__6 s-g-remove-child-margin"
            >
              <div class="s-g-section__card__6__img-box"
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

      <div
              class="s-g-grid__item"
              style="grid-column: 1 / 5"
      >
        <div class="s-g-section__tools-list"
        >
          <div class="s-g-section__tools-list__img-box"></div>
          <div class="s-g-section__tools-list__icon-box"><UIButtonAdd isBlack="{true}" /></div>
          <div class="s-g-section__tools-list__img-box"></div>
          <div class="s-g-section__tools-list__icon-box"><UIButtonAdd isBlack="{true}" /></div>
          <div class="s-g-section__tools-list__img-box"></div>
        </div>
      </div>

      <div
              class="s-g-grid__item"
              style="grid-column: 2 / 4"
      >
        <Card
                styleVariante="is-purple-gradient"
                buttonIconIsBlack="{true}"
                buttonColor="var(--s-color--brown--light)"
        >
          <div slot="recto">
            <div class="s-g-section__card__tools"
            >
              <h3>SYMPHONIE DES MACHINES
                <br/>RISO + OFFSET + TYPO
                <br/>
                <br/>COMBINEZ LES CAPACITÉS DES MACHINES POUR DES RÉSULTATS SUR MESURE</h3>
            </div>
          </div>
          <div slot="verso" class="s-g-remove-child-margin"></div>
        </Card>
      </div>

      <div
              class="s-g-grid__item"
              style="grid-column: 2 / 4"
      >
        <div class="s-g-section__we-work-with">
          <h3 class="s-g-section__we-work-with__title">NOUS TRAVAILLONS AVEC DES&nbsp;MACHINES</h3>
          <div class="s-g-section__we-work-with__logo">
            <img alt="logo heidelberg" src="/assets/logo-heidelberg.svg" />
            <img alt="logo riso" src="/assets/logo-riso.svg" />
            <img alt="logo rotaprint" src="/assets/logo-rotaprint.svg" />
          </div>
        </div>
      </div>


    </div>
  </div>
</section>

<style lang="scss">
  .s-g-section__card__1__facenord {
    position: relative;
    padding: 1rem 1rem 0;

    .s-g-section__card__1__facenord__title {
      margin-bottom: 0;
    }

    .s-g-section__card__1__facenord__img-box {
      position: relative;
      width: 100%;
      padding-top: 100%;
      background: red;

      > img {
        display: block;
        position: absolute;
        top: 0;
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center left;
      }
    }
  }

  .s-g-section__card__2__riso {
    position: relative;
    padding: 0 1rem;

    .s-g-section__card__2__riso__options-box {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 1rem;
    }
  }

  .s-g-section__card__3__heidelberg {
    padding: 0 1rem;

    .s-g-section__card__3__heidelberg__title {
      width: 50%;
      margin: 0 0 1rem;
      color: #3E3C2F;
    }

    .s-g-section__card__3__heidelberg__img-box {
      position: absolute;
      background: red;
      width: 50%;
      height: 100%;
      top: 0;
      right: 0;
    }
  }

  .s-g-section__card__4 {
    padding: 0 1rem;

    .s-g-section__card__4__title {
      position: relative;
      z-index: 10;
    }

    .s-g-section__card__4__img-box {
      background: red;
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      z-index: 0;
    }
  }

  .s-g-section__card__5 {
    padding: 0 1rem;

    .s-g-section__card__5__title {
      position: relative;
      z-index: 10;
    }

    .s-g-section__card__5__img-box {
      background: red;
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      z-index: 0;
    }
  }


  .s-g-section__card__6 {
    padding: 0 1rem 1rem;

    .s-g-section__card__6__title {
      position: relative;
      z-index: 10;
    }

    .s-g-section__card__6__img-box {
      background: red;
      position: relative;
      width: 100%;
      height: 3rem;
    }
  }


  .s-g-section__tools-list {
    display: flex;
    width: calc(100% + 2rem);
    align-items: center;
    margin-left: -1rem;
    margin-right: -1rem;
    margin-bottom: -3rem;
    position: relative;
    z-index: 5;
  }

  .s-g-section__tools-list__img-box {
    height: 10rem;
    background: red;
    width: 100%;
  }

  .s-g-section__tools-list__icon-box {
    width: 1.5rem;
    flex-shrink: 0;
  }

  .s-g-section__card__tools {
    padding: 4rem 2rem 2rem;
    text-align: center;
  }

  .s-g-section__we-work-with {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 100%;

    .s-g-section__we-work-with__title {
      text-align: center;
      color: var(--s-color--grey--dark);
    }

    .s-g-section__we-work-with__logo {
      display: flex;
      gap: 2rem;
      justify-content: center;

      > * {
        display: block;
        height: 2rem;
      }
    }
  }
</style>
