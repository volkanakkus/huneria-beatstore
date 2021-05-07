<template>
  <div class="container">
    <div class="logo">
      <img src="~/assets/logo.png" />
    </div>
    <div class="popular">
      <h2 class="title">Öne Çıkan:</h2>
    </div>

    <div class="beats">
      <Track
        :id="1"
        title="Costa"
        price="150"
        :tags="['120bpm', 'F MINOR']"
        cover-url="1.jpg"
        buy-url="https://iyzi.link/AGZ0cg"
      />
      <Track
        :id="2"
        title="Shine"
        price="150"
        :tags="['150bpm', 'D MINOR']"
        cover-url="2.jpg"
        buy-url="https://iyzi.link/AGZ0dw"
      />
      <Track
        :id="3"
        title="Butterfly"
        price="150"
        :tags="['120bpm', 'C# MINOR']"
        cover-url="3.jpg"
        buy-url="https://iyzi.link/AGZ0fA"
      />
      <Track
        :id="4"
        title="Tenet"
        price="120"
        :tags="['138bpm', 'E MAJOR']"
        cover-url="4.jpg"
        buy-url="https://iyzi.link/AGZ0gQ"
      />
      <Track
        :id="5"
        title="Zimms"
        price="120"
        :tags="['110bpm', 'E MINOR']"
        cover-url="5.jpg"
        buy-url="https://iyzi.link/AGZ0sw"
      />
    </div>
    <div class="popular">
      <h2 class="title">Beatler:</h2>
    </div>

    <div class="beats">
      <Track
        :id="6"
        title="No Stop"
        price="120"
        :tags="['146bpm', 'D MINOR']"
        cover-url="6.jpg"
        buy-url="https://iyzi.link/AGZ0vQ"
      />
      <Track
        :id="7"
        title="Fresh"
        price="120"
        :tags="['150bpm', 'E MINOR']"
        cover-url="7.jpg"
        buy-url="https://iyzi.link/AGZ0wg"
      />
      <Track
        :id="8"
        title="ILL Mind"
        price="100"
        :tags="['140bpm', 'D MINOR']"
        cover-url="8.jpg"
        buy-url="https://iyzi.link/AGZ0xw"
      />
      <Track
        :id="9"
        title="Lighter"
        price="100"
        :tags="['140bpm', 'D MINOR']"
        cover-url="4.jpg"
        buy-url="https://iyzi.link/AGZ0zA"
      />
      <Track
        :id="10"
        title="Orchestra"
        price="100"
        :tags="['130bpm', 'C MINOR']"
        cover-url="10.jpg"
        buy-url="https://iyzi.link/AGZ00Q"
      />
    </div>
    <div class="beats">
      <Track
        :id="11"
        title="Glory"
        price="120"
        :tags="['94bpm', 'E MINOR']"
        cover-url="11.jpg"
        buy-url="https://iyzi.link/AGZ02w"
      />
      <Track
        :id="12"
        title="Neon"
        price="120"
        :tags="['130bpm', 'A# MAJOR']"
        cover-url="12.jpg"
        buy-url="https://iyzi.link/AGZ06g"
      />
      <Track
        :id="13"
        title="Watcher"
        price="120"
        :tags="['140bpm', 'E MINOR']"
        cover-url="13.jpg"
        buy-url="https://iyzi.link/AGZ09A"
      />
      <Track
        :id="14"
        title="Late"
        price="120"
        :tags="['140bpm', 'E MINOR']"
        cover-url="14.jpg"
        buy-url="https://iyzi.link/AGZ0_g"
      />
      <Track
        :id="15"
        title="Scream"
        price="120"
        :tags="['150bpm', 'F MINOR']"
        cover-url="15.jpg"
        buy-url="https://iyzi.link/AGZ1Aw"
      />
    </div>
    <div class="beats">
      <Track
        :id="16"
        title="Gone"
        price="100"
        :tags="['128bpm', 'B MINOR']"
        cover-url="16.jpg"
        buy-url="https://iyzi.link/AGZ1CA"
      />
      <Track
        :id="17"
        title="Fogger"
        price="120"
        :tags="['140bpm', 'C MINOR']"
        cover-url="17.jpg"
        buy-url="https://iyzi.link/AGZ1DQ"
      />
      <Track
        :id="18"
        title="Call"
        price="100"
        :tags="['124bpm', 'G# MINOR']"
        cover-url="18.jpg"
        buy-url="https://iyzi.link/AGZ1Fw"
      />
      <Track
        :id="19"
        title="Psy"
        price="120"
        :tags="['150bpm', 'A MINOR']"
        cover-url="19.jpg"
        buy-url="https://iyzi.link/AGZ1IQ"
      />
      <Track
        :id="20"
        title="Swag"
        price="120"
        :tags="['120bpm', 'G MINOR']"
        cover-url="20.jpg"
        buy-url="https://iyzi.link/AGZ1Jg"
      />
    </div>
    <div class="popular">
      <h2 class="title">Diğer:</h2>
    </div>
    <div class="beats">
      <Track
        :id="21"
        title="Revenge"
        price="80"
        :tags="['130bpm', 'B MINOR']"
        cover-url="21.jpg"
        buy-url="https://iyzi.link/AGZ1MA"
      />
      <Track
        :id="22"
        title="Clouds"
        price="80"
        :tags="['120bpm', 'E MINOR']"
        cover-url="22.jpg"
        buy-url="https://iyzi.link/AGZ1Og"
      />
      <Track
        :id="23"
        title="Switch"
        price="80"
        :tags="['100bpm', 'C# MINOR']"
        cover-url="23.jpg"
        buy-url="https://iyzi.link/AGZ1RA"
      />
      <Track
        :id="24"
        title="Synthetic"
        price="50"
        :tags="['110bpm', 'G MINOR']"
        cover-url="24.jpg"
        buy-url="https://iyzi.link/AGZ1Tg"
      />
      <Track
        :id="25"
        title="Agre"
        price="50"
        :tags="['135bpm', 'A MINOR']"
        cover-url="25.jpg"
        buy-url="https://iyzi.link/AGZ1Uw"
      />
    </div>
    <div class="footer">
      <span>
        Beat önizlemelerinin kalitesi oldukça düşüktür, satın alındığına .wav
        halde teslim edilecektir.</span
      >
      <span class="last"
        ><a href="mailto:prodby@huneria.com">prodby@huneria.com</a> © Tüm
        Hakları Saklıdır</span
      >
    </div>
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

.footer {
  padding: 65px 30px 45px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  color: #948dab;
  font-size: 20px;
  font-weight: 300;
  text-align: center;
}

.footer span {
  display: block;
}

.footer .last {
  padding-top: 13px;
  font-size: 15px;
  font-weight: 500;
}

span.last a:hover {
  color: #fff;
}

.container {
  max-width: 1352px;
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
  padding-top: 10vh;
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
  padding: 6px 7px;
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
  margin-top: 25px;
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
