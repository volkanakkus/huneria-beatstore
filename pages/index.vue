<template>
  <div class="container">
    <div class="logo">
      <img src="~/assets/logo.png" />
    </div>
    <div class="popular">
      <h2 class="title">Popüler Beatler:</h2>
    </div>

    <div class="beats">
      <Track />
      <Track />
      <div class="track">
        <div
          class="player"
          style="background-image: url('~/assets/covers/2.png')"
        >
          <div class="price">75₺</div>
          <progress
            class="amplitude-song-played-progress"
            data-amplitude-song-index="1"
            id="song-played-progress-2"
          ></progress>
          <div class="control-container">
            <div
              class="button amplitude-play-pause"
              data-amplitude-song-index="1"
            ></div>
          </div>
        </div>
        <div class="track-title">Pinky</div>
        <div class="tags"><span>153bpm</span><span>C MINOR</span></div>
        <a class="buy" href="#">
          <div class="cart"></div>
          <span>Satın Al</span>
        </a>
      </div>
      <div class="track">
        <div
          class="player"
          style="background-image: url('~/assets/covers/3.png')"
        >
          <div class="price">75₺</div>
          <progress
            class="amplitude-song-played-progress"
            data-amplitude-song-index="2"
            id="song-played-progress-3"
          ></progress>
          <div class="control-container">
            <div
              class="button amplitude-play-pause"
              data-amplitude-song-index="2"
            ></div>
          </div>
        </div>
        <div class="track-title">POKÊ</div>
        <div class="tags"><span>145bpm</span><span>ENERJIK</span></div>
        <a class="buy" href="#">
          <div class="cart"></div>
          <span>Satın Al</span>
        </a>
      </div>
      <div class="track">
        <div
          class="player"
          style="background-image: url('~/assets/covers/4.png')"
        >
          <div class="price">75₺</div>
          <progress
            class="amplitude-song-played-progress"
            data-amplitude-song-index="3"
            id="song-played-progress-4"
          ></progress>
          <div class="control-container">
            <div
              class="button amplitude-play-pause"
              data-amplitude-song-index="3"
            ></div>
          </div>
        </div>
        <div class="track-title">Wrecked</div>
        <div class="tags"><span>120bpm</span><span>duygusal</span></div>
        <a class="buy" href="#">
          <div class="cart"></div>
          <span>Satın Al</span>
        </a>
      </div>
      <div class="track">
        <div
          class="player"
          style="background-image: url('~/assets/covers/5.png')"
        >
          <div class="price">75₺</div>
          <progress
            class="amplitude-song-played-progress"
            data-amplitude-song-index="4"
            id="song-played-progress-5"
          ></progress>
          <div class="control-container">
            <div
              class="button amplitude-play-pause"
              data-amplitude-song-index="4"
            ></div>
          </div>
        </div>
        <div class="track-title">Fanus</div>
        <div class="tags"><span>120bpm</span><span>duygusal</span></div>
        <a class="buy" href="#">
          <div class="cart"></div>
          <span>Satın Al</span>
        </a>
      </div>
    </div>
    <div class="popular">
      <h2 class="title">Tüm Beatler:</h2>
    </div>

    <div class="beats">
      <div class="track">
        <div
          class="player"
          style="background-image: url('~/assets/covers/1.png')"
        >
          <div class="price">100₺</div>
          <progress
            class="amplitude-song-played-progress"
            data-amplitude-song-index="0"
            id="song-played-progress-1"
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
      <div class="track">
        <div
          class="player"
          style="background-image: url('~/assets/covers/2.png')"
        >
          <div class="price">75₺</div>
          <progress
            class="amplitude-song-played-progress"
            data-amplitude-song-index="1"
            id="song-played-progress-2"
            @click="move(e)"
          ></progress>
          <div class="control-container">
            <div
              class="button amplitude-play-pause"
              data-amplitude-song-index="1"
            ></div>
          </div>
        </div>
        <div class="track-title">Pinky</div>
        <div class="tags"><span>153bpm</span><span>C MINOR</span></div>
        <a class="buy" href="#">
          <div class="cart"></div>
          <span>Satın Al</span>
        </a>
      </div>
      <div class="track">
        <div
          class="player"
          style="background-image: url('~/assets/covers/3.png')"
        >
          <div class="price">75₺</div>
          <progress
            class="amplitude-song-played-progress"
            data-amplitude-song-index="2"
            id="song-played-progress-3"
          ></progress>
          <div class="control-container">
            <div
              class="button amplitude-play-pause"
              data-amplitude-song-index="2"
            ></div>
          </div>
        </div>
        <div class="track-title">POKÊ</div>
        <div class="tags"><span>145bpm</span><span>ENERJIK</span></div>
        <a class="buy" href="#">
          <div class="cart"></div>
          <span>Satın Al</span>
        </a>
      </div>
      <div class="track">
        <div
          class="player"
          style="background-image: url('~/assets/covers/4.png')"
        >
          <div class="price">75₺</div>
          <progress
            class="amplitude-song-played-progress"
            data-amplitude-song-index="3"
            id="song-played-progress-4"
          ></progress>
          <div class="control-container">
            <div
              class="button amplitude-play-pause"
              data-amplitude-song-index="3"
            ></div>
          </div>
        </div>
        <div class="track-title">Wrecked</div>
        <div class="tags"><span>120bpm</span><span>duygusal</span></div>
        <a class="buy" href="#">
          <div class="cart"></div>
          <span>Satın Al</span>
        </a>
      </div>
      <div class="track">
        <div
          class="player"
          style="background-image: url('~/assets/covers/5.png')"
        >
          <div class="price">75₺</div>
          <progress
            class="amplitude-song-played-progress"
            data-amplitude-song-index="4"
            id="song-played-progress-5"
          ></progress>
          <div class="control-container">
            <div
              class="button amplitude-play-pause"
              data-amplitude-song-index="4"
            ></div>
          </div>
        </div>
        <div class="track-title">Fanus</div>
        <div class="tags"><span>120bpm</span><span>duygusal</span></div>
        <a class="buy" href="#">
          <div class="cart"></div>
          <span>Satın Al</span>
        </a>
      </div>
    </div>
  </div>
</template>

<script></script>
