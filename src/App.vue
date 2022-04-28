<template>
  <div class="main">
    <soft-skills/>
    <photo/>
  </div>
</template>

<script>
import Photo from './components/Photo.vue';
import SoftSkills from './components/SoftSkills.vue';

export default {
  components: { SoftSkills, Photo },

  name: 'App',
};
</script>

<style lang="scss">
@import '@/assets/scss/main.scss';

.main {
  background-color: $white;
}
</style>
