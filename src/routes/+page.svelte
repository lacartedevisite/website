<svelte:head>
  <title>La CARTE DE VISITE Genève</title>
  <meta name="description" content="This is where the description goes for SEO" />
</svelte:head>

<div
        class="s-page"
>
  <SectionIntro/>
  <SectionImpression/>
  <SectionGraphisme/>
  <SectionReproduction/>
  <SectionAbout/>


</div>


<script lang="ts">
  import SectionImpression from "$lib/SectionImpression.svelte";
  import SectionGraphisme from "$lib/SectionGraphisme.svelte";
  import SectionReproduction from "$lib/SectionReproduction.svelte";
  import SectionAbout from "$lib/SectionAbout.svelte";
  import SectionIntro from "$lib/SectionIntro.svelte";

</script>
