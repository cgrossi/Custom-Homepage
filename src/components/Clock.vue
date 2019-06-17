<template>
  <div class="clock">
    <h2>{{ clockTime }}</h2>
    <p>{{ date }}</p>
  </div>
</template>

<script>
import moment from "moment";
export default {
  name: "Clock",
  data() {
    return {
      clockTime: null,
      date: null
    };
  },
  created() {
    this.clockTime = moment().format("h:mm a");
    this.date = moment().format("dddd, MMMM Do YYYY");
  }
};
</script>

<style lang="scss">
.clock h2 {
  font-size: 3rem;
  margin-bottom: 12px;
  margin-top: 10px;
}
</style>

