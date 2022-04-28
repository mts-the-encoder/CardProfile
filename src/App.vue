<template>
  <button-hard-skills/>
  <button-soft-skills/>
</template>

<script>
import ButtonHardSkills from './components/ButtonHardSkills.vue';
import ButtonSoftSkills from './components/ButtonSoftSkills.vue';

export default {
  components: { ButtonHardSkills, ButtonSoftSkills },
  name: 'App',
};
</script>

<style lang="scss">
@import '@/assets/scss/main.scss';
</style>
