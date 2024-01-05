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
            >
              <div slot="recto"
                   class="s-section-about__card__assos__recto"
              >
                <p>L’ASSOCIATION</p>
                <h2>PRÉSERVATION, ÉDUCATION, COOPÉRATION: LES PILIERS DE L’ASSOCIATION</h2>
              </div>

              <div slot="verso">
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

              </div>
            </Card>
          </div>
          <div class="s-g-grid__item"
               style="grid-column: 1 / 3"
          >

            <Card
                    styleVariante="is-purple"
            >
              <div slot="recto">
                <h3>PERSONNE RÉFÉRENTE DE L’IMPRIMERIE :</h3>
              </div>
              <div slot="verso"
              >
                <p>
                  Clovis Duran apporte son expertise dans la conception graphique, les outils numériques, la typographie, les techniques d’impression et la micro-éditon.
                  A ses côtés, les autres membres fondateur·rice·s de l’association, Clarisse Coeur et Clément Drévo, apportent des compétences complémentaires en développement d’activités, stratégies et communication L’entourage de l’association est un vivier de spécialistes dans divers domaines qui saura la conseiller afin de faire vivre l’entreprise à la hauteur de ses ambitions.
                </p>
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
          <div slot="recto">
            <p>NOS STATUTS</p>
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
            <h3>VOUS AVEZ UN PROJET ? DISCUTONS-EN!</h3>
            <div
                    class="s-section-about__meeting"
            >
              <a href="mailto:INFO@LACARTEDEVISITE.CH"
                 target="_blank"
                 class="s-g-ui-button"
              >INFO@LACARTEDEVISITE.CH</a>
              <a href="tel:+41223277477"
                 target="_blank"
                 class="s-g-ui-button"
              >+41 22 327 74 77</a>
            </div>
          </div>
          <div slot="verso"
          >
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

<style>
  .s-section-about__card__assos__recto {
      padding-bottom: 10rem;
  }

  .s-section-about__meeting {
      margin-top: 5rem;
  }
</style>
