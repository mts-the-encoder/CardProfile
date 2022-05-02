<template>
  <div class="main">
    <card/>
  </div>
</template>

<script>
import Card from './components/Card.vue';

export default {
  components: { Card },

  name: 'App',
};
</script>

<style lang="scss">
@import '@/assets/scss/main.scss';

.main {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
