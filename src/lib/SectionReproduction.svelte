<script>
import Card from "$lib/Card.svelte";
</script>

<section
        class="s-g-section"
        id="reproduction"
>
  <div class="s-g-section__title"
  >
    <h2>Reproduction</h2>
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
                title="REPRODUCTION"
                titleColor="#646464"
                backgroundFrontCard="transparent conic-gradient(from -90deg at 52% 116%, #B1ADA7 0%, #FFFFFF 100%) 0% 0% no-repeat padding-box"
        >
          <div slot="recto">
            <div class="s-g-section__card__reproduction s-g-remove-child-margin">
              <div class="s-g-section__card__reproduction__img-box"
              >
                <img
                        alt="carte"
                        src="/assets/imgs/carte_detoure.png"
                  />
              </div>
              <h3 class="s-g-font-l s-g-section__card__reproduction__title"
              >PRÉSERVATION ET REPRODUCTION DE QUALITÉ POUR MUSÉES ET COLLECTIONNEUR·SE·S</h3>
            </div>
          </div>
          <div slot="verso" class="s-g-remove-child-margin">
            <h2>Reproduction de documents imprimés pour les musées et les collectionneur·se·s</h2>

            <h3>Préservation des originaux :</h3>
            <p>Permet aux musées et aux collectionneur·se·s de conserver leurs documents précieux en parfait état,
              évitant
              ainsi l'usure due à l'exposition ou à la manipulation grâce à des reproductions de haute qualité.</p>

            <h3>Haute Fidélité :</h3>
            <p>Grâce à notre expertise en traitement d'images, nous garantissons une reproductionau plus proche de
              l’original.</p>

            <h3>Accessibilité et démocratisation :</h3>
            <p>Les reproductions de qualité permettent de partager des documents rares ou fragiles avec un public plus
              large, contribuant ainsi à l'éducation et à la diffusion culturelle.</p>

            <h3>Options de personnalisation :</h3>
            <p>Adaptation flexible du processus de reproduction en fonction des besoins spécifiques de chaque œuvre,
              qu'il s'agisse de la taille, du type de papier ou de la finition.</p>

            <h3>Durabilité :</h3>
            <p>Utilisation de matériaux et d'encres de qualité supérieure pour des impressions qui résistent au temps,
              idéales pour des expositions ou des archives.</p>

            <h3>Un processus méticuleux</h3>
            <p>Que ce soit la couleur, la texture ou la dimension, notre objectif est de capturer l'essence du document
              original. L'impression est ensuite réalisée avec le plus grand soin, en utilisant des techniques et des
              matériaux qui assurent non seulement une fidélité visuelle mais aussi une durabilité. Les musées et les
              collectionneurs bénéficient ainsi d'un service qui respecte l'intégrité de l'original tout en offrant une
              copie idéale pour l'exposition et l'étude.</p>
          </div>
        </Card>
      </div>
    </div>
  </div>
</section>

<style lang="scss">
  .s-g-section__card__reproduction {
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

  .s-g-section__card__reproduction__title {
    width: 50%;
    text-align: center;

    @media (max-width: 860px) {
      width: 100%;
    }
  }
  .s-g-section__card__reproduction__img-box {
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
