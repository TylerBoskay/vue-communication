<template>
  <h3>{{ $store.state.counter }}</h3>
</template>

<script>
export default {
  name: 'TheCounter',
  computed: {
    counter() {
      return this.$store.state.getters.finalCounter;
    }
  }
};
</script>

<style scoped>

</style>