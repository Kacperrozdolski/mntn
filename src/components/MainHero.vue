<template>
  <section>
    <nav>
      <h1 class="logo">MNTN</h1>
      <div class="menu">
        <p>Equipment</p>
        <p>About us</p>
        <p>Blog</p>
      </div>
      <div class="account">
        Account <img src="../assets/userIcon.svg" alt="" srcset="" />
      </div>
    </nav>
    <main>
      <div class="hero-content">
        <p>hiking guide</p>
        <h1>Be prepared for The Mountains and beyond!</h1>
        <div @click="scrollDown"></div>
        <span>scroll</span>
      </div>
    </main>
  </section>
</template>

<script>
export default {
  name: "MainHero",
  methods: {
    scrollDown() {
      window.scroll({
        top: 700,
        behavior: "smooth",
      });
    },
  },
};
</script>

<style lang="scss" scoped>
section {
  background: url("../assets/heroBackground.jpg");
  min-height: 100vh;
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
    .account {
      display: flex;
      align-items: center;
      gap: 10px;
    }
  }
  main {
    min-height: 100vh;
    display: flex;
    align-items: center;
    flex-direction: column;
    width: 90%;
    .hero-content {
      margin-top: 10%;
      height: 30%;
      width: 50%;
      display: flex;
      flex-direction: column;
      position: relative;
      p {
        margin: 0;
        font-family: Poppins;
        position: relative;
        color: #545764;
        padding-left: 12%;
      }
      p::before {
        position: absolute;
        content: "";
        background: #545764;
        width: 10%;
        height: 3px;
        left: 0;
        top: calc(50% - 2px);
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
        cursor: pointer;
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

@media only screen and (max-width: 600px) {
  section {
    nav {
      justify-content: center;
      .menu {
        display: none;
      }
      .account {
        display: none;
      }
      .logo {
        font-size: 5.5rem;
        margin: 20px;
      }
    }
    main {
      width: 100%;
      .hero-content {
        width: 100%;
        justify-content: center;
        align-items: center;
        margin: 0;
        h1 {
          max-width: 90%;
          margin: 40px;
          font-size: 10vw;
          text-align: center;
        }
        p {
          padding: 0;
        }
        p::before {
          margin: 0;
          padding: 0;
          display: none;
        }
      }
    }
  }
}
</style>
