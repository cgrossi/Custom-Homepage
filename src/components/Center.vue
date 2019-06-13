<template>
  <div class="center third wrapper">
    <HelloCarmine/>
    <Clock/>
  </div>
</template>

<script>
import HelloCarmine from "./HelloCarmine";
import Clock from "./Clock";
export default {
  name: "Center",
  components: {
    HelloCarmine,
    Clock
  }
};
</script>

<style lang="scss">
</style>
