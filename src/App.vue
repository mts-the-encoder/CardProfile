<template>
  <div class="main">
    <soft-skills/>
    <contact/>
  </div>
</template>

<script>
import Contact from './components/Contact.vue';
import SoftSkills from './components/SoftSkills.vue';

export default {
  components: { SoftSkills, Contact },

  name: 'App',
};
</script>

<style lang="scss">
@import '@/assets/scss/main.scss';

.main {
  background-color: $white;
}
</style>
