<template>
  <div class="app">
    <main>
      <Left/>
      <Center/>
      <Right/>
    </main>
    <Footer></Footer>
  </div>
</template>

<script>
import Right from "./components/Right";
import Left from "./components/Left";
import Center from "./components/Center";
import Footer from "./components/Footer";

export default {
  name: "app",
  components: {
    Right,
    Left,
    Center,
    Footer
  }
};
</script>

<style lang="scss">
*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff;
  height: 100vh;
  width: 100vw;
  background-image: url("./assets/Moraine-Lake.jpg");
  background-size: cover;
  background-position: center top;
  background-repeat: no-repeat;
}

// .app div {
//   border: 1px solid red;
// }

main {
  display: flex;
  height: 85%;
  margin-bottom: 15px;
}

main .center {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

// .hello {
//   background-color: rgba(48, 57, 75, 0.767);
//   border-radius: 3px;
// }

.third {
  width: 33.3333%;
  height: 100%;
}

.wrapper {
  padding: 30px;
}

.app .footer {
  width: 100vw;
  height: 70px;
  border: 1px solid red;
  color: rgb(228, 228, 228);
}
</style>
