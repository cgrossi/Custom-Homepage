<template>
  <div class="hello">
    <h1>{{ current }} Carmine</h1>
  </div>
</template>

<script>
import moment from "moment";
export default {
  name: "HelloCarmine",
  data() {
    return {
      greeting: {
        morning: "Good Morning",
        afternoon: "Good Afternoon",
        evening: "Good Evening"
      },
      current: null
    };
  },
  created() {
    let time = +moment().format("H");
    if (time < 12) {
      this.current = this.greeting.morning;
    } else if (time < 16) {
      this.current = this.greeting.afternoon;
    } else {
      this.current = this.greeting.evening;
    }
  }
};
</script>

<style lang="scss">
.hello h1 {
  font-size: 2.5rem;
}
</style>
