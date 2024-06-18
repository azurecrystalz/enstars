---
title: Trip Album
date: 2023-05-30 19:30:00
categories:
- [Enstars , Crazy:B]
tags:
- Songs
description: trip album song list
---

<style>
.stories {
    display: grid;
    grid-template-columns: repeat(auto-fill,minmax(150px,1fr));
    gap: .5em
}

.stories * {
    box-sizing: border-box
}

.story {
    position: relative;
    border-radius: .25em;
    overflow: hidden !important
}

.stories a:hover {
    color: #fff !important
}

.story:hover img {
    transform: scale(1.05)
}

.story:hover .storyName {
    transform: translate(0,0)
}

.story:hover .storyName .read {
    transform: translate(0,0)
}

.storyName {
    transform: translate(0,0)
}

.image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: .2s ease;
    margin: 0!important
}

.storyName {
    font-size: .9em;
    font-weight: 700;
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
    background: linear-gradient(to bottom,transparent 0,#000000a3 90%) !important;
    color: #fff !important;
    position: absolute;
    padding: 5em .75em .75em !important;
    width: 100%;
    bottom: 0;
    left: 0;
    transition: .2s ease !important;
    transform: translate(0,2.3em)
}

.storyName .read {
    margin-top: .25em;
    font-size: .85em;
    background: #000;
    color: #fff;
    padding: .5em 1.25em;
    height: 2.25em;
    border-radius: .25em;
    width: 100%;
    text-align: center;
    transition: .2s ease;
    transform: translate(0,1em)
}

.storyName .read:before {
    content: "Read"
}

.storyName .read.soon {
    opacity: .5;
    pointer-events: none
}

.storyName .read:not(.soon):hover {
    color: #F486AA
}

@keyframes rotate {
  0% {transform: rotate(0)}
  25% {transform: rotate(90deg)}
  50% {transform: rotate(180deg)}
  75% {transform: rotate(270deg)}
  100% {transform: rotate(360deg)}
}

#songs {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-column-gap: 15px;
}

#songs .song-item {
  width: 200px;
}

#songs .song-figure {
  position: relative;
  width: 200px;
  height: 200px;
  border-radius: 50%;
  overflow: hidden;
  margin-block-start: 0em;
  margin-inline-start: 0px;
}

#songs .song-figure .song-image {
  width: 200px;
  height: 200px;
  border-radius: 50%;
  transition: transform 1.33s, filter: 0.2s;
}

#songs .song-figure .song-image.rotate {
  animation: rotate 12s linear 0s infinite forwards;
}

#songs .song-figure .song-caption:link, #songs .song-figure .song-caption:visited {
  color: var(--V98);
}

#songs .song-figure:hover > .song-image {
  filter: blur(4px);
}

#songs .song-figure .song-caption {
  position: absolute;
  visibility: hidden;
  display: grid;
  align-items: center;
  justify-content: center;
  top: 50%;
  left: 50%;
  transform: translate(-49%, -49%);
  z-index: 5;
  width: 180px;
  height: 180px;
  border-radius: 50%;
  background-color: rgba(0, 0, 0, 0.5);
  text-align: center;
}

#songs .song-figure:hover > .song-caption {
  visibility: visible;
}

@media only screen and (max-width: 600px) {
    .stories {
        grid-template-columns:repeat(auto-fill,minmax(100px,1fr))
    }

    #songs {
      grid-template-columns: 1fr;
      justify-content: center;
    }

    #songs .song-item {
      width: 100%;
      margin-bottom: 5%;
    }

    #songs .song-figure {
      margin: auto;
      width: 60vw;
      height: 60vw;
    }

    #songs .song-figure .song-image {
      width: 100%;
      height: 100%;
    }

    #songs .song-figure .song-caption {
      visibility: visible;
      width: 80vw;
      height: 80vw;
    }
}
@import url('https://fonts.googleapis.com/css?family=Cardo:400i|Rubik:400,700&display=swap');

  :root {
    --d: 700ms;
    --e: cubic-bezier(0.19, 1, 0.22, 1);
    --font-sans: 'Rubik', sans-serif;
    --font-serif: 'Cardo', serif;
  }

  * {
    box-sizing: border-box;
  }

  html,
  body {
    height: 100%;
  }

  body {
    display: grid;
    place-items: center;
  }

  .page-content {
    padding: 1rem;
    font-family: var(--font-sans);
  }
  .grid-container {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 1%;
  }
  .item {
    position: relative;
    color: white;
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center center;
    overflow: hidden;
    border-radius: 10px;
    font-size: 0.8rem;
    height: 300px;
    cursor: pointer;
    display: block;
    margin: 0;
  }
  .item::before {
    position: absolute;
    content: "";
    display: block;
    width: 100%;
    height: 100%;
    background: linear-gradient(transparent, #000000bb);
  }
  .item-container-link {
    position: absolute;
    z-index: 2;
    display: block;
    height: 100%;
    transform: translateY(20px);
  }
  a:link.item-container-link, a:visited.item-container-link {
    z-index: 2;
    color: white;
    transition: transform 0.3s;
  }
  a:hover.item-container-link, a:active.item-container-link {
    z-index: 2;
    background: none;
  }
  .item-container {
    height: 100%;
    display: flex;
    flex-flow: column nowrap;
    align-items: center;
    justify-content: flex-end;
    padding: 1px 5px 5px 10px;
    box-sizing: border-box;
  }
  .read {
    display: block;
    width: 100%;
    text-decoration: none;
    text-align: center;
    background: black;
    color: white;
    height: 20px;
    border-radius: 3px;
    font-weight: 600;
  }
  .item:hover a:link.item-container-link, .item:hover a:visited.item-container-link, .item:hover a:active.item-container-link, .item:hover a:hover.item-container-link {
    /* hover effect */
    transform: translateY(2px);
  }

  @media (max-width: 768px) {
    .grid-container {
      display: block;
    }
    .item {
      display: flex;
      align-items: center;
      justify-content: flex-end;
      margin-bottom: 2%;
      background-position-y: 20%;
      height: 100px;
    }
    .item-container-link {
      transform: translateY(0);
    }
    .title h2 {
      margin:0;
      margin-bottom:5px;
    }
    .item::before {
      background-image: linear-gradient(to right, transparent, #000000bb);
    }
    .item-container {
      width: 100%;
      transform: translateY(12px);
    }
    .title {
      text-align: right;
      margin-right: 3px;
    }
  }
</style>

<sup><i><b>NOTE:</b> I try to follow the cadence of the song while still staying true to the lyrics, so translations may deviate from the concrete meaning.</i></sup>

<main class="page-content">
  <h2>Idol Solos</h2>
  <strong><p><i>Everything is complete unless marked with "WIP"/"Unadded" !!</i></p></strong>
  <!-- other things can go in this div -->
  <div class="grid-container">
    <!-- copy and paste this if you need more grids for other translation categories-->
    <div class="item" id="rinne" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706325660/translation%20site/masterlist/ye1ftcktglgw5yiw0ja9.png');">
      <a href="/2023/05/22/thrill-addict/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>Thrill Addict</h2>
          </div>
        </div>
      </a>
    </div>
    <div class="item" id="himeru" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706325658/translation%20site/masterlist/zlitxwgl8vxnjpwkaaim.webp');">
      <a href="/2023/05/22/shisen-hold-me-tight/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>視線 Hold me Tight</h2>
          </div>
        </div>
      </a>
    </div>
    <div class="item" id="niki" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706325664/translation%20site/masterlist/sk9nq5sxhe2emu6mpbr9.png');">
      <a href="/2023/08/01/yummy-tummy-love/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>Yummy・Tummy・LOVE !!</h2>
          </div>
        </div>
      </a>
    </div>
    <div class="item" id="kohaku" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706325658/translation%20site/masterlist/adigi7l32tpp6cykgzwt.webp');">
      <a href="/2023/05/22/petals-resolution/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>Petal's Resolution</h2>
          </div>
        </div>
      </a>
    </div>
  </div>
  <!-- more translation categories can go here -->
  <h2>Unit Album Songs</h2>
  <!-- other things can go in this div -->
  <div class="grid-container">
    <!-- copy and paste this if you need more grids for other translation categories-->
    <div class="item" id="kurei" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706326199/translation%20site/masterlist/gzvbbtyfpckiwkxisyue.png');">
      <a href="/2023/05/30/crazy-anthem/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>Crazy Anthem</h2>
          </div>
        </div>
      </a>
    </div>
    <div class="item" id="kurei" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706402122/translation%20site/masterlist/drsaldpl0rrsyybcqa2o.png');">
      <a href="/2023/05/22/summer-night-beat/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>NA NA NA SUMMER NIGHT BeeAT</h2>
          </div>
        </div>
      </a>
    </div>
</main>