<template>
  <div class="right third wrapper">
    <Weather/>
  </div>
</template>

<script>
import Weather from "./WeatherComponent";
export default {
  name: "Right",
  components: {
    Weather
  }
};
</script>