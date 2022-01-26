<template>
<button @click='addTwo'>Add 2</button>
</template>

<script>
export default {
  name: 'ChangeCounter.vue',
  methods: {
    addTwo() {
      // Different ways to commit data using a Mutation //
      // this.$store.commit('increment') // Using the mutation name
      // this.$store.commit('increase', 2); // Using Name, and Payload
      //this.$store.commit('increment', { value: 10 }); // Using Name, and Payload Value Object
      this.$store.commit({ // Using Object with type, and payload.
        type: 'increment',
        payload: { value: 10 }
      });
    }
  }
};
</script>

<style scoped>

</style>