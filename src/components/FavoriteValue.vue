<template>
<div>
  <h3>{{ counter }}</h3>
  <p>We do more..</p>
</div>
</template>

<script>
export default {
  name: 'FavoriteValue',
  computed: {
    counter() {
      return this.$store.getters.normalizedCounter;
    }
  }
};
</script>

<style scoped>

</style>