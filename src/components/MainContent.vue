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
          <span>read more</span>
        </div>
      </div>
      <div class="content-image">
        <img src="../assets/contentImage_01.png" alt="" srcset="" />
      </div>
    </div>
    <div class="content-card">
      <div class="content-image">
        <img src="../assets/contentImage_02.png" alt="" srcset="" />
      </div>
      <div class="content-text">
        <div class="text right">
          <p class="subtitle">HIKING ESSENTIALS</p>
          <h1>Picking the right Hiking Gear!</h1>
          <p>
            The nice thing about beginning hiking is that you don’t really need
            any special gear, you can probably get away with things you already
            have. Let’s start with clothing. A typical mistake hiking beginners
            make is wearing jeans and regular clothes, which will get heavy and
            chafe wif they get sweaty or wet.
          </p>
          <span>read more</span>
        </div>
      </div>
    </div>
    <div class="content-card">
      <div class="content-text">
        <div class="text">
          <p class="subtitle">WHERE YOU GO IS THE KEY</p>
          <h1>Understand Your Map & Timing</h1>
          <p>
            To start, print out the hiking guide and map. If it’s raining, throw
            them in a Zip-Lock bag. Read over the guide, study the map, and have
            a good idea of what to expect. I like to know what my next landmark
            is as I hike. For example, I’ll read the guide and know that say, in
            a mile, I make a right turn at the junction..
          </p>
          <span>read more</span>
        </div>
      </div>
      <div class="content-image">
        <img src="../assets/contentImage_03.png" alt="" srcset="" />
      </div>
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
  align-items: center;
  padding: 100px 0;
  flex-direction: column;
  gap: 100px;

  .content-card {
    height: 720px;
    width: 80%;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;

    .content-text {
      width: 55%;
      height: 100%;
      display: flex;
      justify-content: center;
      flex-direction: column;
      .right {
        align-self: flex-end;
      }
      .text {
        display: flex;
        flex-direction: column;
        width: 80%;
        height: 60%;
        .subtitle {
          position: relative;
          margin: 0 !important;
        }
        h1 {
          margin: 0 0 5% 0;
          font-size: 4em;
        }
        p {
          margin: 0 0 5% 0;
          padding: 0;
          font-family: Poppins;
        }
        span {
          font-family: Poppins;
        }
      }
    }
    .content-image {
      width: 45%;
      height: 100%;
      background: grey;
      img {
        width: 100%;
        height: 100%;
      }
    }
  }
}
</style>
