<template>
  <section>
    <nav>
      <h1 class="logo">MNTN</h1>
      <div class="menu">
        <p>Equipment</p>
        <p>About us</p>
        <p>Blog</p>
      </div>
      <div class="account">Account</div>
    </nav>
    <main>
      <div class="hero-content">
        <p>A hiking guide</p>
        <h1>
          Be prepared for The<br />
          Mountains and beyond!
        </h1>
        <div></div>
        <span>scroll</span>
      </div>
    </main>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
section {
  background: url("../assets/heroBackground2.jpg");
  height: 100vh;
  background-size: cover;
  width: 100%;
  background-position: center;
  display: flex;
  align-items: center;
  flex-direction: column;
  color: white;

  nav {
    width: 90%;
    height: 20%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-family: Poppins;
    .menu {
      display: flex;
      flex-direction: row;
      gap: 20px;
    }
  }
  main {
    height: 100%;
    display: flex;
    align-items: center;
    flex-direction: column;
    width: 90%;
    .hero-content {
      margin-top: 10%;
      height: 30%;
      display: flex;
      flex-direction: column;
      position: relative;
      p {
        margin: 0;
        font-family: Poppins;
      }
      h1 {
        font-size: 4rem;
        margin: 0 0 20px 0px;
      }
      span {
        color: #d3d3d3d8;
        align-self: center;
        font-family: Poppins;
      }
      div {
        width: 20px;
        min-height: 40px;
        border-radius: 40px;
        border: 2px solid #d3d3d3d8;
        align-self: center;
        position: relative;
      }
      div::before {
        position: absolute;
        top: 10px;
        left: 50%;
        content: "";
        width: 3px;
        height: 3px;
        margin-left: -1px;
        background-color: #d3d3d3d8;
        -webkit-animation: sdb10 2s infinite;
        animation: sdb10 2s infinite;
      }
      @-webkit-keyframes sdb10 {
        0% {
          -webkit-transform: translate(0, 0);
          opacity: 0;
        }
        40% {
          opacity: 1;
        }
        80% {
          -webkit-transform: translate(0, 20px);
          opacity: 0;
        }
        100% {
          opacity: 0;
        }
      }
      @keyframes sdb10 {
        0% {
          transform: translate(0, 0);
          opacity: 0;
        }
        40% {
          opacity: 1;
        }
        80% {
          transform: translate(0, 20px);
          opacity: 0;
        }
        100% {
          opacity: 0;
        }
      }
    }
  }
}
</style>
