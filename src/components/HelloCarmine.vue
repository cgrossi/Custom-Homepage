<template>
  <div class="hello">
    <h1>Hello, Carmine</h1>
  </div>
</template>

<script>
export default {
  name: "HelloCarmine",
  data() {
    return {
      greeting: [
        { morning: "Good Morning" },
        { afternoon: "Good Afternoon" },
        { evening: "Good Evening" }
      ]
    };
  },
  props: {}
};
</script>

<style lang="scss">
</style>
