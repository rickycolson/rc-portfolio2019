<template>
  <div class="container content">
    <h1 class="title is-1">Cabells</h1>
    <h3 class="subtitle">Designer, Project Manager, UI/UX, Content Strategist/Copywriter, User Researcher; UI/UX Design, Product Design, Print Design, Data Vis, Marketing, Copywriting</h3>
    <section class="content">
      <p>
          This is an explanation of my roles at Cabells. It contains a an overview of what I did there and the areas I covered.
      </p>
    </section>
    <CabellsProject/>
  </div>
</template>

<script>
import CabellsProject from "@/components/CabellsProject.vue"

export default {
  name: 'Cabells',
  components: {
    CabellsProject
  }
}
</script>
