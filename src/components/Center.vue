<template>
  <div class="center third wrapper">
    <div class="hello-container">
      <HelloCarmine/>
      <Clock/>
    </div>
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
// .center {
//   padding: 30px;
// }

.hello-container {
  padding: 30px;
  background-color: rgba(48, 57, 75, 0.5);
  border-radius: 2px;
}
</style>
