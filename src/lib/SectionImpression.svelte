<script>
import Card from "$lib/Card.svelte";
</script>

<section
        class="s-g-section"
>
  <h2
          class="s-g-section__title"
  >IMPRESSION</h2>
  <div>
    <div>
      <Card
      >
        <div slot="recto" >
          <p class="s-g-font-xxl">hello</p>
        </div>
        <div slot="verso" >verso</div>
      </Card>
    </div>
  </div>
</section>
