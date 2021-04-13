<template>
  <section>
    <div class="content-card">
      <div class="content-text">
        <div class="text">
          <p class="subtitle">GET STARTED</p>
          <h1>What level of hiker are you?</h1>
          <p>
            Determining what level of hiker you are can be an important tool
            when planning future hikes. This hiking level guide will help you
            plan hikes according to different hike ratings set by various
            websites like All Trails and Modern Hiker. What type of hiker are
            you – novice, moderate, advanced moderate, expert, or expert
            backpacker?
          </p>
          <a href="https://modernhiker.com/" target="_blank">read more</a>
        </div>
      </div>
      <img src="../assets/contentImage_01.jpg" alt="" srcset="" />
    </div>
    <div class="content-card">
      <div class="content-text">
        <div class="text">
          <p class="subtitle">HIKING ESSENTIALS</p>
          <h1>Picking the right Hiking Gear!</h1>
          <p>
            The nice thing about beginning hiking is that you don’t really need
            any special gear, you can probably get away with things you already
            have. Let’s start with clothing. A typical mistake hiking beginners
            make is wearing jeans and regular clothes, which will get heavy and
            chafe wif they get sweaty or wet.
          </p>
          <a
            href="https://www.rei.com/learn/expert-advice/hot-weather-hiking.html"
            target="_blank"
            >read more</a
          >
        </div>
      </div>
      <img src="../assets/contentImage_02.png" alt="" srcset="" />
    </div>
    <div class="content-card">
      <div class="content-text">
        <div class="text">
          <p class="subtitle">WHERE YOU GO IS THE KEY</p>
          <h1>What level of hiker are you?</h1>
          <p>
            To start, print out the hiking guide and map. If it’s raining, throw
            them in a Zip-Lock bag. Read over the guide, study the map, and have
            a good idea of what to expect. I like to know what my next landmark
            is as I hike. For example, I’ll read the guide and know that say, in
            a mile, I make a right turn at the junction..
          </p>
          <a
            href="https://www.thehikinglife.com/hiking-and-backpacking-skills/navigation/"
            target="_blank"
            >read more</a
          >
        </div>
      </div>
      <img src="../assets/contentImage_03.png" alt="" srcset="" />
    </div>
  </section>
</template>

<script>
export default {
  name: "MainContent",
};
</script>

<style lang="scss" scoped>
section {
  min-height: 100vh;
  width: 100%;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  .content-card:nth-child(2) {
    flex-direction: row-reverse;
    .content-text {
      justify-content: flex-end;
    }
  }
  .content-card {
    min-height: 520px;
    margin: 30px 0px;
    display: flex;
    align-items: center;
    flex-direction: row;
    width: 80%;
    .content-text {
      width: 65%;
      min-height: 100%;
      display: flex;
      justify-content: flex-start;
      align-items: center;
      .text {
        width: 69%;
        min-height: 100%;
        .subtitle {
          font-family: Poppins;
          position: relative;
          padding-left: 15%;
          font-weight: 500;
        }
        .subtitle::before {
          position: absolute;
          content: "";
          background: #545764;
          width: 10%;
          height: 3px;
          left: 0;
          top: calc(50% - 2px);
        }
        h1 {
          font-size: 3rem;
          margin: 0;
        }
        p {
          font-family: Poppins;
        }
        a {
          font-family: Poppins;
          font-weight: 300;
          text-decoration: none;
          color: inherit;
        }
      }
    }
    img {
      max-width: 45%;
      max-height: 100%;
    }
  }
}

@media only screen and (max-width: 900px) {
  section {
    .content-card {
      width: 95%;
      flex-direction: column !important;
      justify-content: center !important;
      align-items: center !important;
      gap: 20px;
      .content-text {
        min-width: 100%;
        justify-content: center !important;
        .text {
          width: 95%;
        }
      }
      img {
        max-width: 100%;
        min-height: 100%;
      }
    }
  }
}
</style>
