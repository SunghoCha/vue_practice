<template>
  <button @click="addOne">Add 10</button>
</template>

<script>
  export default {
    methods: {
      addOne() {
        //this.$store.commit('increment');
        //this.$store.commit('increase', {value: 10});
        this.$store.commit({
          type: 'increase',
          value: 10
        });
      }
    }
  }
</script>

<style lang="scss" scoped>

</style>