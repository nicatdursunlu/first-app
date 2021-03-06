<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <h1>Hello, {{ name }}</h1>
  <h2 v-text="job" v-bind:id="jobID"></h2>
  <button v-bind:disabled="disabled">Click me</button>
  <h3 class="underline">Underline text</h3>
  <h3 class="underline" v-bind:class="status">Status</h3>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      name: "Nijat Dursunlu",
      job: "Front-End | Mobile Developer",
      disabled: false,
      jobID: "job-id",
      status: "danger",
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.underline {
  text-decoration: underline;
  color: blueviolet;
}
</style>
