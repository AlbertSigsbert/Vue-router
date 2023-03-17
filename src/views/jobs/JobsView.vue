<template>
  <h1>Jobs</h1>
  <div v-for="job in jobs" :key="job.id">
    {{ job.title }}
  </div>
</template>

<script>
export default {
  data() {
    return {
      jobs: [
        {
          id: 1,
          title: "Software Engineer",
          salary: 100000,
          location: "Seattle, WA",
        },
        {
          id: 2,
          title: "Data Analyst",
          salary: 80000,
          location: "New York, NY",
        },
        {
          id: 3,
          title: "Product Manager",
          salary: 120000,
          location: "San Francisco, CA",
        },
        {
          id: 4,
          title: "UX Designer",
          salary: 90000,
          location: "Los Angeles, CA",
        },
        {
          id: 5,
          title: "Marketing Manager",
          salary: 110000,
          location: "Chicago, IL",
        },
      ],
    };
  },
};
</script>

<style>
</style>