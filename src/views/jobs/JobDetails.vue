<template>
  <h1>{{job.title}}</h1>
  <p>Job Id is {{ id }}</p>
  <p>Salary: {{ job.salary}}</p>
  <p>Location: {{ job.location }}</p>
</template>

<script>
export default {
  props: ["id"],
  data() {
    return {
      job:null,
    };
  },

  mounted() {
    fetch("http://localhost:3000/jobs/"+this.id)
      .then((res) => res.json())
      .then((data) => (this.jobs = data))
      .catch((err) => console.log(err.message));
  },
};
</script>

<style>
</style>