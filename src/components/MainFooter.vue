<template>
  <footer>
    <div class="asd">
      <h2>MNTN</h2>
      <p>
        Get out there & discover your next slope,<br />
        mountain & destination!
      </p>
      <span>Copyright 2019 MNTN, Inc. Terms & Privacy</span>
    </div>
    <div class="asd1">
      <h2>More on The Blog</h2>
      <p>About MNTN</p>
      <p>Contributors & Writers</p>
      <p>Write For Us</p>
      <p>Contact Us</p>
      <p>Privacy Policy</p>
    </div>
    <div class="asd2">
      <h2>More on MNTN</h2>
      <p>The Team</p>
      <p>Jobs</p>
      <p>Press</p>
    </div>
  </footer>
</template>

<script>
export default {
  name: "MainFooter",
};
</script>

<style lang="scss" scoped>
footer {
  min-height: 30vh;
  width: 80%;
  display: flex;
  font-family: Poppins;
  padding-bottom: 5vh;
  .asd {
    width: 55%;
    min-height: 100%;
    display: flex;
    flex-direction: column;
    p {
      margin: 0;
    }
    span {
      margin-top: auto;
    }
  }
  .asd1 {
    width: 25%;
    height: 100%;
  }
  .asd2 {
    min-width: 20%;
    min-height: 100%;
  }
}
</style>
