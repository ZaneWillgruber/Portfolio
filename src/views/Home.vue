<template>
  <div class="home">
    <section class="hero">
      <div class="hero-text container">
        <h4>Computer Scientist</h4>
        <hr />
        <h2>ZANE WILLGRUBER</h2>
      </div>
    </section>
  </div>
  <section>
    <div class="container-fluid">
      <div class="row">
        <div style="background-color: #7c9eb2" class="col-sm">
          <div class="row d-flex">
            <div class="peice-content">
              <img src="@/assets/friendSoup.png">
              <a href="https://hacketthuntergmailcom.itch.io/friendsoup" target="_blank" rel="noopener noreferrer"><button type="button" class="btn btn-light"><i class="fa-brands fa-itch-io"></i>Itch.io Page</button></a>
            </div>
          </div>
        </div>
        <div style="background-color: #c2eaba" class="col-sm">
          <div class="row d-flex">
            <div class="peice-content">
              <img src="@/assets/partyHouseSimulator.png">
              <a href="https://authenticchops.itch.io/party-house-simulator" target="_blank" rel="noopener noreferrer"><button type="button" class="btn btn-light"><i class="fa-brands fa-itch-io"></i>Itch.io Page</button></a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
// @ is an alias to /src
export default {
  name: "HomeView",
  components: {},
};
</script>

<style lang="scss" scoped>
@import url("https://www.dafontfree.net/embed/Y2VudHVyeS1nb3RoaWMtYm9sZCZkYXRhLzQ3L2MvNTA3NjIvZ290aGljYi50dGY");

.row {
  height: 100vh;
}

.hero {
  background-color: #feefd7;
  //background-image: url("../assets/hero-bg.jpg");
  background-attachment: fixed;
  background-size: cover;
  position: relative;
  width: 100%;
  height: 100vh;
  img {
    object-fit: cover;
    height: 50%;
    width: 50%;
  }
  .hero-text {
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    color: #f15a29;
    font-weight: bold;
    h4 {
      text-transform: uppercase;
      font-size: 22px;
      padding-bottom: 4px;
    }
    h2 {
      font-family: "century-gothic-bold", sans-serif;
      font-size: 50px;
      @media (min-width: 550px) {
        font-size: 80px;
      }
    }
    hr:nth-child(2) {
      max-width: 365px;
      margin-bottom: 16px;
    }
    hr:nth-child(4) {
      height: 6px;
      background-color: #fff;
      border: none;
      max-width: 85px;
      margin-top: 16px;
    }
  }
}

.peice-content {
 display: flex;
  justify-content: center;
  align-items: center;
}
</style>