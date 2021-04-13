<template>
  <div class="mntn-body">
    <MainHero />
    <MainContent />
    <MainFooter />
  </div>
</template>

<script>
import MainHero from "./components/MainHero";
import MainContent from "./components/MainContent";
import MainFooter from "./components/MainFooter";
export default {
  name: "App",
  components: { MainHero, MainContent, MainFooter },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Poppins&display=swap");
body {
  margin: 0 !important;
}
.mntn-body {
  min-height: 100vh;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
</style>
