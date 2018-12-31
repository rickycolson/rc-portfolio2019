<template>
  <section class="container content">
    <h1 class="title is-2 is-spaced">Cabells</h1>
    <p class="subtitle is-4"><strong>Roles:</strong> Designer, Project Manager, Content Strategist/Copywriter, User Researcher, Data Specialist</p>
    <div class="content">
      <p>
          This is an explanation of my roles at Cabells. It contains a an overview of what I did there and the areas I covered.
      </p>
    </div>
    <CabellsProject/>
  </section>
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
