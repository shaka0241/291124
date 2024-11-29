<script>
import Presentation from './components/Presentation.vue';
import Education from './components/Education.vue';
import WorkExperience from './components/WorkExperience.vue';
export default {
  name: 'App',
  components: {
    Presentation,
    Education,
    WorkExperience
  }
}
</script>

<template>
<div id="app">
  <main>
    <Presentation />
    <Education />
    <WorkExperience />
  </main>
</div>
</template>

<style scoped>
</style>
