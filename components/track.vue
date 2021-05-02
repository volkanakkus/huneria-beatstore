<template>
  <div class="track">
    <div
      class="player"
      :style="{
        backgroundImage: 'url(' + require('@/assets/covers/' + coverUrl) + ')'
      }"
    >
      <div class="price">{{ price }}₺</div>
      <progress
        class="amplitude-song-played-progress"
        :data-amplitude-song-index="id - 1"
        :id="'song-played-progress-' + id"
        @click="move"
      ></progress>
      <div class="control-container">
        <div
          class="button amplitude-play-pause"
          :data-amplitude-song-index="id - 1"
        ></div>
      </div>
    </div>
    <div class="track-title">{{ title }}</div>
    <div v-if="tags.length > 0" class="tags">
      <span v-for="(tag, index) in tags" :key="index">{{ tag }}</span>
    </div>
    <a class="buy" :href="buyUrl" target="_blank">
      <div class="cart"></div>
      <span>Satın Al</span>
    </a>
  </div>
</template>

<script>
import Amplitude from "amplitudejs";
import songs from "../helpers/songs";

export default {
  props: {
    id: {
      type: Number,
      required: true
    },
    title: {
      type: String,
      required: true
    },
    price: {
      type: String,
      required: true
    },
    tags: {
      type: Array
    },
    coverUrl: {
      type: String,
      required: true
    },
    buyUrl: {
      type: String,
      required: true
    }
  },
  mounted() {
    Amplitude.init(songs);
  },
  methods: {
    move(e) {
      if (Amplitude.getActiveIndex() == this.id - 1) {
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
