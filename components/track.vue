<template>
  <div class="track">
    <div
      class="player"
      :style="{
        backgroundImage: 'url(' + require('@/assets/covers/1.png') + ')'
      }"
    >
      <div class="price">100₺</div>
      <progress
        class="amplitude-song-played-progress"
        data-amplitude-song-index="0"
        id="song-played-progress-1"
        @click="move"
      ></progress>
      <div class="control-container">
        <div
          class="button amplitude-play-pause"
          data-amplitude-song-index="0"
        ></div>
      </div>
    </div>
    <div class="track-title">Ballon</div>
    <div class="tags"><span>120bpm</span><span>duygusal</span></div>
    <a class="buy" href="#">
      <div class="cart"></div>
      <span>Satın Al</span>
    </a>
  </div>
</template>

<script>
import Amplitude from "amplitudejs";
import songs from "../helpers/songs";

export default {
  mounted() {
    Amplitude.init(songs);
  },
  methods: {
    move(e) {
      if (Amplitude.getActiveIndex() == 0) {
        var offset = e.target.getBoundingClientRect();
        var x = e.pageX - offset.left;

        Amplitude.setSongPlayedPercentage(
          (parseFloat(x) / parseFloat(e.target.offsetWidth)) * 100
        );
      }
    }
  }
};
</script>

<style lang="scss" scoped></style>
