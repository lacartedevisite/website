<section
        class="s-section-about s-g-section"
        id="about"
>
  <div class="s-g-section__title"
  >
    <h2>À Propos</h2>
  </div>
  <div
          class="s-g-section__content"
  >
    <div class="s-g-grid s-g-grid--coll-4"
    >
      <div class="s-g-grid__item"
           style="grid-column: 1 / 3"
      >

        <div class="s-g-grid s-g-grid--coll-2"
        >
          <div class="s-g-grid__item"
               style="grid-column: 1 / 3"
          >
            <Card
                    styleVariante="is-green"
                    buttonColor="#814DF5"
            >
              <div slot="recto"
                   class="s-section-about__card__assos__recto"
              >
                <p>L’ASSOCIATION</p>
                <h2>PRÉSERVATION, ÉDUCATION, COOPÉRATION: LES&nbsp;PILIERS DE L’ASSOCIATION</h2>
              </div>

              <div slot="verso" class="s-g-remove-child-margin">
                <p>Raison d’être de l’association: « préserver, valoriser, faire valoir et développer l’art et les
                  techniques associés à l’impression artisanale et à l’édition »</p>
                <p>Notamment grâce à :</p>
                <p>L’opérationnalisation d’imprimeries artisanales</p>
                <ul>
                  <li>L’acquisition, la gestion et la maintenance de machines et d’outils d’impression</li>
                  <li>La sensibilisation et la formation aux techniques et aux méthodes d’impressions</li>
                  <li>La production, reproduction et l’édition de projet faisant une part centrale à l’impression</li>
                  <li>La production de commun dans une démarche de libre accès</li>
                  <li>La recherche et le développement de techniques, de gestes et d’outils innovants</li>
                </ul>

                <p>L’association La Carte de visite refuse toute discrimination d’ordre politique, religieux ou racial.
                  Son fonctionnement repose sur un système de valeurs partagées et de collaboration.</p>

                <p>Membres de l’association :</p>

                <ul>
                  <li>Clovis Duran,</li>
                  <li>Clément Drévo,</li>
                  <li>Clarisse Coeur.</li>
                  <li>Isabelle Vaudaux,</li>
                  <li>Nicolas Baldran</li>
                </ul>

                <a class="s-g-ui-button"
                        target="_blank"
                   href="/assets/status-v202311.pdf"
                >Status format PDF</a>

              </div>
            </Card>
          </div>
          <div class="s-g-grid__item"
               style="grid-column: 1 / 3"
          >

            <Card
                    styleVariante="is-purple"
                    buttonColor="#3E3C2F"
            >
              <div class="s-section-about__card__person-ref__recto"
                      slot="recto">
                <h3>PERSONNE RÉFÉRENTE<br>DE L’IMPRIMERIE :</h3>
                <p>CLOVIS DURAN</p>
              </div>
              <div slot="verso" class="s-g-remove-child-margin"
              >
                <p>
                  Clovis Duran apporte son expertise dans la conception graphique, les outils numériques, la typographie, les techniques d’impression et la micro-éditon.
                </p>
                <p>A ses côtés, les membres fondateur·rice·s de l’association, Clarisse Coeur et Clément Drévo, apportent des compétences complémentaires en développement d’activités, stratégies et communication.</p>
              </div>
            </Card>
          </div>
        </div>
      </div>

      <div class="s-g-grid__item"
           style="grid-column: 3 / 5"
      >
        <Card
                styleVariante="is-grey"
        >
          <div class="s-section-about__card__status__recto"
               slot="recto">
            <p>NOS STATUTS</p>

            <div class="s-section-about__card__status__recto__img-box"
            >
              <img src="/assets/imgs/association_visuel.jpg"
                   alt="illustration du document pour les status"
              />
              <a class="s-g-ui-button"
                 target="_blank"
                 href="/assets/status-v202311.pdf"
                 style="color: black; display: block; margin-top: 3rem"
              >Status format PDF</a>
            </div>
          </div>



        </Card>
      </div>

      <div class="s-g-grid__item"
           style="grid-column: 1 / 5"
      >
        <img alt="intérieur de l'imprimerie"
             src="/photo_matos.png"
             style="display: block; width: 100%; border-radius: var(--s-radius)"
        />
      </div>

      <div class="s-g-grid__item"
           style="grid-column: 1 / 5"
      >
        <Map/>
      </div>

      <div class="s-g-grid__item"
           style="grid-column: 1 / 5"
      >

        <Card
                styleVariante="is-yellow"
        >
          <div slot="recto">
            <div
                    class="s-section-about__meeting s-g-remove-child-margin"
            >
              <h3 class="s-section-about__meeting__title"
              >VOUS AVEZ UN PROJET ? DISCUTONS-EN!</h3>

              <div class="s-section-about__meeting__content"
              >
                <a href="mailto:clovis@lacartedevisite.ch"
                   target="_blank"
                   class="s-g-ui-button"
                >clovis@lacartedevisite.ch</a>
                <a href="tel:+41223287477"
                   target="_blank"
                   class="s-g-ui-button"
                >+41 22 328 74 77</a>
              </div>
            </div>
          </div>
        </Card>
      </div>
    </div>
  </div>
</section>


<script lang="ts">
import Map from "$lib/Map.svelte";
import Card from "$lib/Card.svelte";
</script>

<style lang="scss">
  .s-section-about__card__assos__recto {
    padding: 1rem 1rem 10rem 1rem;
  }

  .s-section-about__meeting {
    display: flex;
    flex-direction: column;
    padding: 1rem;
  }

  .s-section-about__meeting__title {
    width: 100%;
    margin-bottom: 4rem;

    @media (max-width: 860px) {
      margin-bottom: 2rem;
    }
  }

  .s-section-about__meeting__content {
    display: flex;
    gap: 1rem;
    flex-direction: row;

    @media (max-width: 860px) {
      flex-direction: column;
    }
  }

  .s-section-about__card__person-ref__recto {
    padding: 1rem;
    min-height: 10rem;
    display: flex;
    justify-content: center;
    flex-direction: column;
  }

  .s-section-about__card__status__recto {
    padding: 1rem;
  }

  .s-section-about__card__status__recto__img-box {
    width: 100%;
    padding: 2rem;
    box-sizing: border-box;

    > img {
      display: block;
      width: 100%;
      height: auto;
    }
  }
</style>
