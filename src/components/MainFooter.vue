<template>
  <footer>
    <div class="copyright">
      <h2>MNTN</h2>
      <p>
        Get out there & discover your next slope,<br />
        mountain & destination!
      </p>
      <span>Copyright 2019 MNTN, Inc. Terms & Privacy</span>
    </div>
    <div class="blog">
      <h2>More on The Blog</h2>
      <p>About MNTN</p>
      <p>Contributors & Writers</p>
      <p>Write For Us</p>
      <p>Contact Us</p>
      <p>Privacy Policy</p>
    </div>
    <div class="more">
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
  gap: 25px;
  padding-bottom: 5vh;
  .copyright {
    width: 60%;
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
  .blog {
    width: 30%;
    min-height: 100%;
    display: flex;
    flex-direction: column;
    gap: 15px;
    h1 {
      margin: 0;
    }
    p {
      margin: 0;
    }
  }
  .more {
    width: 20%;
    min-height: 100%;
    display: flex;
    flex-direction: column;
    gap: 15px;
    h1 {
      margin: 0;
    }
    p {
      margin: 0;
    }
  }
}
@media only screen and (max-width: 900px) {
  footer {
    width: 95%;
    font-size: 0.7rem;
  }
}
@media only screen and (max-width: 454px) {
  footer {
    flex-direction: column;
    .copyright {
      width: 100%;
    }
    .blog {
      width: 100%;
    }
    .more {
      width: 100%;
    }
  }
}
</style>
