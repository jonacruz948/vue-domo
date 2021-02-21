<template>
  <v-container>
    <v-row>
      <v-col cols="12" md="10" offset-md="1" class="container">
        <v-img class="anim" src="../assets/animation.gif">
          <!-- <v-container fluid class="fill-height px-4"> -->
          <div class="col-md-4 my-span marquee bottom-centered display-1">
            <span>{{ marquee_text }}</span>
          </div>
          <!-- </v-container> -->
        </v-img>
      </v-col>
      <v-row class="text-center">
        <v-col cols="12">
          <v-btn color="red" outlined> Subscribe for Updates</v-btn>
        </v-col>
      </v-row>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    timer: null,
    marquee_text: null,
    dataArray: ["A canary network", "Polkadot experiment"],
  }),
  methods: {
    start() {
      this.isRunning = true;
      if (!this.timer) {
        this.timer = setInterval(() => {
          if (this.time > 0) {
            this.time--;
          } else {
            clearInterval(this.timer);
            this.reset();
          }
        }, 1000);
      }
    },
    stop() {
      this.isRunning = false;
      clearInterval(this.timer);
      this.timer = null;
    },
    reset() {
      this.stop();
    },
    setTime(payload) {
      this.time = payload.minutes * 60 + payload.secondes;
    },
  },
};
</script>

<style>
.anim {
  display: inline-block;
  width: 100%;
  height: auto;
  max-width: 768px;
}
.my-span {
  /* background-color: blue; */
  color: white;
  font-weight: bold;
  margin-right: 0;
}

/* Container holding the image and the text */
.container {
  position: relative;
  text-align: center;
  color: white;
}

/* Bottom left text */
.bottom-left {
  position: absolute;
  bottom: 8px;
  left: 16px;
}

/* Top left text */
.top-left {
  position: absolute;
  top: 10%;
  left: -10%;
  display: inline-block;
}

/* Top right text */
.top-right {
  position: absolute;
  top: 8px;
  right: 16px;
}

/* Bottom right text */
.bottom-right {
  position: absolute;
  bottom: 10px;
  right: 16px;
}

/* Centered text */
.centered {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.bottom-centered {
  position: absolute;
  bottom: 10px;
  left: 50%;
  transform: translate(-50%, -50%);
}

.marquee {
  margin: 0 auto;
  white-space: nowrap;
  overflow: hidden;
  position: absolute;
}

.marquee span {
  display: inline-block;
  padding-left: 100%;
  animation: marquee 10s linear infinite;
}

.marquee2 span {
  animation-delay: 2.5s;
}

@keyframes marquee {
  0% {
    transform: translate(0, 0);
  }
  100% {
    transform: translate(-100%, 0);
  }
}
</style>
