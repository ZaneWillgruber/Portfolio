<template>
  <div class="home">
    <section class="hero">
      <div class="hero-text container">
        <h4>
          Computer
          <span class="typed-text">{{ typeValue }}</span>
          <span class="cursor" :class="{ typing: typeStatus }">&nbsp;</span>
        </h4>
        <hr />
        <h2>
          <a
            href="https://www.linkedin.com/in/zane-willgruber/"
            target="_blank"
            rel="noopener noreferrer"
            >ZANE WILLGRUBER</a
          >
        </h2>
      </div>
    </section>
  </div>
  <section>
    <div class="container-fluid">
      <div class="row">
        <div style="background-color: #7c9eb2" class="col-sm">
          <div class="row d-flex">
            <div class="peice-content">
              <img src="@/assets/friendSoup.png" />
              <a
                href="https://hacketthuntergmailcom.itch.io/friendsoup"
                target="_blank"
                rel="noopener noreferrer"
                ><button type="button" class="btn btn-light">
                  <i class="fa-brands fa-itch-io"></i>Itch.io Page
                </button></a
              >
            </div>
          </div>
        </div>
        <div style="background-color: #c2eaba" class="col-sm">
          <div class="row d-flex">
            <div class="peice-content">
              <img src="@/assets/partyHouseSimulator.png" />
              <a
                href="https://authenticchops.itch.io/party-house-simulator"
                target="_blank"
                rel="noopener noreferrer"
                ><button type="button" class="btn btn-light">
                  <i class="fa-brands fa-itch-io"></i>Itch.io Page
                </button></a
              >
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
  data: () => {
    return {
      typeValue: "",
      typeStatus: false,
      typeArray: ["Scientist", "Wizard", "Lover", "Gamer"],
      typingSpeed: 200,
      erasingSpeed: 100,
      newTextDelay: 2000,
      typeArrayIndex: 0,
      charIndex: 0,
    };
  },
  methods: {
    typeText() {
      if (this.charIndex < this.typeArray[this.typeArrayIndex].length) {
        if (!this.typeStatus) {
          this.typeStatus = true;
        }
        this.typeValue += this.typeArray[this.typeArrayIndex].charAt(
          this.charIndex
        );
        this.charIndex += 1;

        setTimeout(this.typeText, this.typingSpeed);
      } else {
        this.typeStatus = false;
        setTimeout(this.eraseText, this.newTextDelay);
      }
    },
    eraseText() {
      if (this.charIndex > 0) {
        if (!this.typeStatus) {
          this.typeStatus = true;
        }

        this.typeValue = this.typeArray[this.typeArrayIndex].substring(
          0,
          this.charIndex - 1
        );
        this.charIndex -= 1;
        setTimeout(this.eraseText, this.erasingSpeed);
      } else {
        this.typeStatus = false;
        this.typeArrayIndex += 1;
        if (this.typeArrayIndex >= this.typeArray.length)
          this.typeArrayIndex = 0;

        setTimeout(this.typeText, this.typingSpeed + 1000);
      }
    },
  },
  created() {
    setTimeout(this.typeText, this.newTextDelay + 200);
  },
};
</script>

<style lang="scss" scoped>
@import url("https://www.dafontfree.net/embed/Y2VudHVyeS1nb3RoaWMtYm9sZCZkYXRhLzQ3L2MvNTA3NjIvZ290aGljYi50dGY");

html,
body {
  overflow-x: hidden;
}
body {
  position: relative;
}

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

    span.cursor {
      display: inline-block;
      margin-left: 3px;
      width: 2px;
      background-color: #000;
      animation: cursorBlink 1s infinite;
    }

    span.cursor.typing {
      animation: none;
    }
  }

  @keyframes cursorBlink {
    49% {
      background-color: #000;
    }
    49% {
      background-color: transparent;
    }
  }

  h2 {
    font-family: "century-gothic-bold", sans-serif;
    font-size: 50px;
    @media (min-width: 550px) {
      font-size: 80px;
    }
    a {
      color: inherit;
      text-decoration: inherit;
    }
    hr:nth-child(2) {
      max-width: 365px;
      margin-bottom: 16px;
    }
  }
}

.peice-content {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>