<template>
  <div>
    <Nuxt />
  </div>
</template>

<style>
body {
  background: linear-gradient(99.97deg, #1c1d24 -4.87%, #261f38 107.43%);
  font-family: "Roboto", sans-serif;
  color: #fff;
}

body * {
  transition: 0.2s;
}

.container {
  max-width: 1300px;
  margin: auto;
  padding: 0px 26px;
}

.logo {
  display: flex;
  width: 100%;
  justify-content: center;
  margin-top: 13vh;
}

.title {
  font-weight: 300;
  font-size: 35px;
}

.popular {
  padding-top: 8vh;
}

progress.amplitude-song-played-progress:not([value]) {
  background-color: rgb(0 0 0 / 50%);
}

progress.amplitude-song-played-progress {
  background-color: rgb(0 0 0 / 50%);

  -webkit-appearance: none;
  -moz-appearance: none;
  appearance: none;
  width: 100%;
  height: 8px;
  display: block;
  cursor: pointer;
  border-radius: 3px;
  border: none;
}

progress[value="0"] {
  background: transparent;
}

progress[value]::-webkit-progress-bar {
  background-color: rgb(0 0 0 / 50%);
  height: 8px;
  border-radius: 3px;
}

progress[value]::-moz-progress-bar {
  background-color: #d7dee3;
  height: 8px;
  border-radius: 3px;
}

progress[value]::-webkit-progress-value {
  background-color: #d7dee3;
  height: 8px;
  border-radius: 3px;
}

.track {
  max-width: 210px;
  margin-bottom: 40px;
}

.player {
  width: 210px;
  height: 210px;
  position: relative;
  border-radius: 9px 9px 5px 5px;
  display: flex;
  justify-content: flex-end;
  align-items: flex-end;
  background-size: cover;
}

.price {
  position: absolute;
  background: hsl(0deg 0% 0% / 50%);
  display: block;
  padding: 10px 8px 8px;
  border-radius: 7px;
  right: 5%;
  top: 5%;
  font-size: 14px;
  font-weight: 500;
  line-height: 14px;
  transition: 0ms;
  z-index: 99;
}

.player progress {
  width: 100%;
  bottom: 0px;
  padding: 4px;
  border: none;
  display: block;
  padding: 0;
  z-index: 99;
}

.track-title {
  font-size: 21px;
  line-height: 21px;
  font-weight: 300;
  margin-top: 18px;
}

.tags {
  margin-top: 15px;
  display: flex;
}

.tags span {
  display: block;
  background: rgb(255 255 255 / 5%);
  font-size: 13px;
  padding: 7px;
  margin-right: 10px;
  color: rgb(255 255 255 / 68%);
  border-radius: 10px;
  text-transform: uppercase;
  font-weight: 500;
  cursor: pointer;
}

.tags span:hover {
  background: rgb(255 255 255 / 9%);
}

a.buy {
  display: block;
  text-decoration: none !important;
  color: #fff;
  margin-top: 18px;
  background: rgb(255 255 255 / 5%);
  border-radius: 11px;
  font-size: 15px;
  font-weight: 500;
  text-align: center;
  max-width: 210px;
  width: 210px;
  height: 35px;
  position: relative;
  line-height: 36px;
}

a.buy .cart {
  background-color: rgb(255 255 255 / 5%);
  display: block;
  height: 35px;
  width: 35px;
  position: absolute;
  border-radius: 11px;
  background-repeat: no-repeat;
  background-position: 9px;
  background-image: url("~assets/assets/cart.svg");
}

a.buy:hover {
  background: #493b6f;
}

.player:hover .button {
  opacity: 1;
}

.button {
  cursor: pointer;
  opacity: 0;
  display: block;
  width: 100%;
  height: 100%;
  background: #0000007d;
  z-index: 0;
  border-radius: 9px 9px 5px 5px;
  background-image: url("~assets/assets/pause.svg");
  background-repeat: no-repeat;
  background-position: center;
  position: absolute;
  top: 0;
  transition: 0.1s;
}

.button.amplitude-paused {
  background-image: url("~assets/assets/play.svg");
}

.beats {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}

.control-container {
  position: absolute;
  top: 0;
  width: 100%;
  height: 100%;
}

@media screen and (max-width: 500px) {
  .track,
  .player,
  a.buy {
    max-width: 100%;
    width: 100%;
  }
  .player {
    height: 300px;
  }

  a.buy {
    height: 40px;
    line-height: 41px;
  }
  a.buy .cart {
    height: 40px;
    width: 40px;
    background-position: 12px;
  }
}

@media screen and (max-width: 917px) and (min-width: 697px) {
  .beats::after {
    content: "";
    max-width: 210px;
    flex: 1;
  }
}
</style>
