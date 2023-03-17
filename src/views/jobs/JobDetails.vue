<template>
  <h1>Job Details</h1>
  <p>Job Id is {{ id }}</p>
</template>

<script>
export default {
  data() {
    return {
      id: this.$route.params.id,
    };
  },
};
</script>

<style>
</style>