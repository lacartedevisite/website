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
            <h2>Services d'impression Risograph à la pointe de la technologie :</h2>
            <p>Riso MH9350, la machine qui incarne un équilibre parfait entre artisanat traditionnel et technologie de
              pointe. Économique sans sacrifier la qualité, elle offre des impressions en ton direct écologique grâce à
              ses encres à base de soja. Elle est conçue pour minimiser la consommation d'énergie et l'utilisation de
              matériaux polluants. Avec notre duplicateur, nous garantissons la meilleure qualité d'image possible sur
              machine Riso.</p>
            <p>Caractère Artisanal:</p>
            <p>La presse Riso apporte un toucher artisanal à l'impression qui est difficile à reproduire avec des
              méthodes plus industrielles. Chaque tirage est unique, reflétant l'engagement et le savoir-faire qui
              entrent dans sa création.</p>
            <p>La Riso offre la possibilité de combiner les capacités des différentes machines de l’atelier pour des
              résultats sur mesure. Cela permet, par exemple, une couverture avec dorure à chaud et un corps d’ouvrage
              imprimé à la Riso.</p>
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
              >
                <img src="/assets/imgs/chassis_platine_typographique.png" />
              </div>
            </div>
          </div>
          <div slot="verso" class="s-g-remove-child-margin">
            <h2>Presse Heidelberg</h2>
            <p>La carte de visite a réussi à marier le meilleur des deux mondes : l'authenticité de l'impression
              typographique et les avantages des nouvelles technologies. La presse Heidelberg, bien que traditionnelle
              dans son essence, est complétée par un ensemble d'outils numériques qui permettent une grande précision et
              flexibilité. Les techniques modernes d’impression numérique ne peuvent simplement pas égaler le niveau de
              qualité d'une impression typographique et son foulage si caractéristique.</p>
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
              >
                <img src="/assets/imgs/Aa_gaufrage_v3.jpg"
                     alt="illustration gaufrage"
                >
              </div>
            </div>
          </div>
          <div slot="verso" class="s-g-remove-child-margin">
            <h2>Gaufrage : L’art du relief dans vos créations imprimées</h2>
            <p>Vous cherchez à donner une nouvelle dimension à vos projets d'impression ? Explorez notre service spécialisé de gaufrage, une technique qui ajoute texture et profondeur à vos imprimés, en créant un effet de volume.</p>
            <p>Le gaufrage est un procédé artisanal qui consiste à presser une matrice sur un support papier pour y créer une empreinte en relief. Que vous souhaitiez mettre en valeur une image sur une carte de visite ou ajouter une finition élégante à une invitation spéciale, le gaufrage apporte une touche tactile et visuelle unique.</p>
            <p>N'hésitez pas à nous contacter pour découvrir comment le gaufrage peut transformer vos projets d'impression .Nous vous guidons et vous aidons à réaliser vos projets.</p>
          </div>
        </Card>
      </div>



      <div
              class="s-g-grid__item"
              style="grid-column: 4 / 5"
      >
        <Card
                styleVariante='is-image--dark'
                title="OFFSET"
        >
          <div slot="recto">
            <div class="s-g-section__card__5 s-g-remove-child-margin"
            >
              <h3 class="s-g-font-l s-g-section__card__5__title"
              >L’impression offset une couleur format A4</h3>
              <div class="s-g-section__card__5__img-box"
              >
                <img src="/assets/imgs/rotaprint_r40_impression_image_degrade_noir.jpg" />
              </div>
            </div>
          </div>
          <div slot="verso" class="s-g-remove-child-margin">
            <p>La Rotaprint R40, avec sa stature de petite presse Offset, se présente comme une solution d'impression à la fois précise et de haute qualité. Cette machine est particulièrement adapté aux projets qui nécessitent une impression en une ou deux couleurs Pantone.</p>
            <p>Sa capacité à gérer des petits formats, allant jusqu'au A4, la rend idéale pour des travaux d'impression soignés et précis. De plus, cette presse est spécialement conçue pour des tirages de faible à moyen volume, ce qui la rend particulièrement efficace pour des projets où la quantité ne doit pas compromettre la qualité.</p>
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
              >
                <img src="/assets/imgs/impression_a_chaud_detoure.png"
                     alt="impression à chaud"
                >
              </div>
            </div>
          </div>
          <div slot="verso" class="s-g-remove-child-margin">
            <p>Si vous recherchez une finition exceptionnelle pour vos projets d'impression, l'impression à chaud est la
              solution parfaite. Cette technique artisanale ajoute raffinement et sophistication aux cartes de visite,
              aux invitations, et aux petites brochures.</p>
            <p>L'impression à chaud est une méthode artisanale qui consiste à appliquer une feuille métallique ou un
              film sur une surface imprimée en utilisant une plaque chauffée. Le résultat ? Un design brillant et
              texturé qui attire l'œil et élève la qualité perçue de vos imprimés.</p>
          </div>
        </Card>
      </div>

      <div
              class="s-g-grid__item"
              style="grid-column: 1 / 5"
      >
        <div class="s-g-section__tools-list s-remove-mobile-on-version"
        >
          <div class="s-g-section__tools-list__img-box">
            <img src="/assets/imgs/rotaprintR40_1.png"
                 alt="rotaprint R40"
            />
          </div>
          <div class="s-g-section__tools-list__icon-box"><UIButtonAdd isBlack="{true}" /></div>
          <div class="s-g-section__tools-list__img-box">
            <img src="/assets/imgs/risomh9350_2.png"
                 alt="risomh 9350"
            />
          </div>
          <div class="s-g-section__tools-list__icon-box"><UIButtonAdd isBlack="{true}" /></div>
          <div class="s-g-section__tools-list__img-box">
            <img src="/assets/imgs/heidelberg_3.png"
                 alt="offset heidelberg"
            />
          </div>
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
          <div slot="verso" class="s-g-remove-child-margin">
            <div>
              <p>Grâce aux possibilités offertes par nos différentes presses, nous pouvons combiner les capacités des machines pour des résultats sur mesure. Nous pouvons réaliser par exemple, une couverture avec dorure à chaud avec un corps d’ouvrage imprimé à la Riso. Cette approche vous permet d’explorer des territoires graphiques encore inexplorés.</p>
              <p>Artistes, graphistes, créateur·rice·s… : bienvenu·e·s !</p>

              <p>NOUS TRAVAILLONS AVEC DES MACHINES
                <br>ROTAPRINT  RISO  ORIGINAL HEIDELBERG</p>

            </div>
          </div>
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
      width: 50%;
      height: 100%;
      top: 0;
      right: 0;

      > img {
        display: block;
        width: 100%;
        height: 100%;
        object-fit: contain;
      }
    }
  }

  .s-g-section__card__4 {
    padding: 0 1rem;

    .s-g-section__card__4__title {
      position: relative;
      z-index: 10;
      color: black;
      padding-bottom: 6rem;
    }

    .s-g-section__card__4__img-box {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      z-index: 0;

      img {
        display: block;
        width: 100%;
        height: 100%;
        object-fit: cover;
      }
    }
  }

  .s-g-section__card__5 {
    padding: 0 1rem;

    .s-g-section__card__5__title {
      position: relative;
      z-index: 10;
      color: #E0D7C4;
      padding-bottom: 6rem;
    }

    .s-g-section__card__5__img-box {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      z-index: 0;

      > img {
        display: block;
        width: 100%;
        height: 100%;
        object-fit: cover;
      }
    }
  }


  .s-g-section__card__6 {
    padding: 0 1rem 1rem;

    .s-g-section__card__6__title {
      position: relative;
      z-index: 10;
    }

    .s-g-section__card__6__img-box {
      position: relative;
      width: 100%;
      padding-top: 10%;

      > img {
        position: absolute;
        top: 0;
        left: 0;
        display: block;width: 100%;
        height: 100%;
        object-fit: contain;
      }
    }
  }


  .s-g-section__tools-list {
    display: flex;
    width: calc(100% + 2rem);
    align-items: center;
    margin-left: -1rem;
    margin-right: -1rem;
    margin-bottom: -6rem;
    position: relative;
    z-index: 5;
  }

  .s-g-section__tools-list__img-box {
    width: 100%;

    > img {
      display: block;
      width: 100%;
      height: auto;
    }
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
