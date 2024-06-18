---
title: Masterlist
date: 2023-05-22 21:50:01
description: translation masterlist
---

<style>

.other-item{
  position: relative;
}

.otherstory-title{
  font-size:20px;
}

.newholder {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
}

.newfeature{
  border-radius: 5px;
  padding: 5px;
  transition: transform .1s;
}

.newfeature:hover {
  transform: scale(1.03);
}

.newfeature img{
  max-width: 135px;
  max-height: 135px;
}

.stories {
    display: grid;
    grid-template-columns: repeat(auto-fill,minmax(175px,1fr));
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
  @media only screen and (max-width: 600px) {
    .newholder {
      grid-template-columns:repeat(auto-fill, minmax(200px,1fr))
    }
  }
</style>

<div style="margin-top: 3%">
  <style>
    .hint--error.hint--top-left:before, .hint--error.hint--top-right:before, .hint--error.hint--top:before {
    border-top-color: #6a3446;
    }
    .hint--error:after {
    background-color: #6a3446;
    text-shadow: 0 -1px 0px #592726;
    }
    [character] {
      --dark-mode: hsl(var(--hue), 30%, 30%);
      display: flex;
    }
    [character]::before {
      position: absolute;
      margin-left: 75px;
    }
    [character] p {
      max-width: calc(100% - 75px);
      margin-left: 75px;
      color: inherit;
    }
    :root[theme='dark'] [character] p {
      background: var(--dark-mode);
    }
    :root[theme='dark'] [character] p .thought {
      color: #9f9fff;
    }
    :root[theme='light'] [character] p {
      background: var(--light-mode);
    }
    [character] p:first-child {
      margin-top: 20px;
      border-top-left-radius: 0px;
    }
    [character] p:first-child::before {
      position: absolute;
      left: 0;
    }
    [character]::after {
      display: none;
      left: 65px;
      top: 37px;
    }
    .msr-narration {
      display: flex;
      align-items: center;
      margin: 20px 0px;
      gap: 5px;
    }
    .msr-narration::before {
      content: "";
      display: inline-block;
      background: var(--article-text);
      height: 1px;
      width: 15%;
    }
    .msr-narration p {
      margin: 0;
    }
    @media (max-width: 650px) {
    [character] p {
        margin:0 0 .4em 65px;
        padding: .72em;
        margin-left: 55px !important;
    }
    [character]::before,[character][hidden]::before,[character][unknown]::before {
        margin-left: 70px;
        margin-left: 55px !important;
    }
}
.article-entry img, .article-entry video {
    margin-bottom: -1em;
}
  </style>

<strong><p><i>Everything is complete unless marked with "WIP"/"Unadded" !!</i></p></strong>
<main class="page-content">
  <!-- other things can go in this div -->
  <h2>Featured Scout Stories: Series 1</h2>
  <div class="grid-container">
    <!-- copy and paste this if you need more grids for other translation categories-->
    <div class="item" id="rinne" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706322603/translation%20site/masterlist/dniwfmzfzsjylrdmkhd7.webp');">
      <a href="/2050/07/05/bees-knees/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>The Bees Knees</h2>
          </div>
        </div>
      </a>
    </div>
    <div class="item" id="himeru" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706322756/translation%20site/masterlist/pexigkzcejb1n4iaosn3.png');">
      <a href="/2050/07/05/past-present-and/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>Past, Present, And...</h2>
          </div>
        </div>
      </a>
    </div>
    <div class="item" id="niki" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706322602/translation%20site/masterlist/x58zlxrww39tpurqlrkj.webp');">
      <a href="/2050/07/05/recipe-for-idols/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>A Recipe for Idols</h2>
          </div>
        </div>
      </a>
    </div>
    <div class="item" id="kohaku" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706322849/translation%20site/masterlist/ijrxend3aknjsd80io9h.png');">
      <a href="/2050/05/24/sakura-sakura/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>Sakura, Sakura</h2>
          </div>
        </div>
      </a>
    </div>
  </div>
  <h2>Featured Scout Stories: Series 2</h2>
  <!-- other things can go in this div -->
  <div class="grid-container">
    <!-- copy and paste this if you need more grids for other translation categories-->
    <div class="item" id="rinne" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706322603/translation%20site/masterlist/x1ab8y3skibltxtdg8ab.webp');">
      <a href="/2050/07/05/new-game-making-the-rounds/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>A New Game Making the Rounds (Unadded)</h2>
          </div>
        </div>
      </a>
    </div>
    <div class="item" id="himeru" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706324123/translation%20site/masterlist/tpviy8cxcxl0cvnjpz7w.png');">
      <a href="/2050/07/05/composed-moment/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>A Composed Moment</h2>
          </div>
        </div>
      </a>
    </div>
    <div class="item" id="niki" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706323119/translation%20site/masterlist/qlpszm1yy4pd72f5q4qc.png');">
      <a href="/2050/05/22/bon-appetit/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>Bon Appetit!</h2>
          </div>
        </div>
      </a>
    </div>
    <div class="item" id="kohaku" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1714609050/translation%20site/masterlist/tlvdgegkhlggsa99jyvt.png');">
      <a href="/2050/07/05/dear-someone-i-dont-know/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>Dear Someone I Don't Know (Unadded)</h2>
          </div>
        </div>
      </a>
    </div>
  </div>
  <h2>Event Stories</h2>
  <!--- aaaa --->
  <div class="grid-container">
    <!-- copy and paste this if you need more grids for other translation categories-->
    <div class="item" id="rinne" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706323977/translation%20site/masterlist/amdarqrjuw0a4xxrtqxq.png');">
      <a href="/2050/05/30/number-eight/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>Number Eight (WIP)</h2>
          </div>
        </div>
      </a>
    </div>
    <div class="item" id="kohaku" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706323992/translation%20site/masterlist/o3vya2vd23733dvho8ha.png');">
      <a href="/2050/05/27/spider-direc/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>Spider</h2>
          </div>
        </div>
      </a>
    </div>
    </div>
    <h2>Themed Scout Stories: Series 1</h2>
  <!--- aaaa --->
  <div class="grid-container">
    <!-- copy and paste this if you need more grids for other translation categories-->
    <div class="item" id="HiMERU" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706322603/translation%20site/masterlist/yums1dnylph0vkvaoznz.webp');">
      <a href="/2050/07/03/rom-date/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>Romantic? Date</h2>
          </div>
        </div>
      </a>
    </div>
    </div>
    <h2>Themed Scout Stories: Series 2</h2>
  <!--- aaaa --->
  <div class="grid-container">
    <!-- copy and paste this if you need more grids for other translation categories-->
    <div class="item" id="rinne" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706323074/translation%20site/masterlist/or06kbz1407iwsbey3uo.png');">
      <a href="/2050/11/03/moon-banquet/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>Banquet Under a Shrouded Moon (WIP)</h2>
          </div>
        </div>
      </a>
    </div>
    </div>
    <h2>ES 4* Scout Stories: Series 2</h2>
  <!-- other things can go in this div -->
  <div class="grid-container">
    <!-- copy and paste this if you need more grids for other translation categories-->
    <div class="item" id="rinne" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706322994/translation%20site/masterlist/nkpiavlwllrptyq9tk5o.png');">
      <a href="/2050/05/16/please-god/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>Please, God ☆</h2>
          </div>
        </div>
      </a>
    </div>
    <div class="item" id="himeru" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706322950/translation%20site/masterlist/so6ancjsdlreh8powmbc.png');">
      <a href="/2050/05/15/runrun-calamity/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>The Runrun Calamity</h2>
          </div>
        </div>
      </a>
    </div>
    <div class="item" id="niki" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706323147/translation%20site/masterlist/ztqchdz31nswmgvr1c6q.png');">
      <a href="/2050/05/15/sweetsroad/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>Sweets Road</h2>
          </div>
        </div>
      </a>
    </div>
    <div class="item" id="kohaku" style="background-image: url('https://res.cloudinary.com/djq41tb84/image/upload/v1706322939/translation%20site/masterlist/t0xdln29oz34ndj6kuud.png');">
      <a href="/2050/05/21/a-curious-step-forward/" class="item-container-link">
        <div class="item-container">
          <div class="title">
            <h2>A Curious Step Forward</h2>
          </div>
        </div>
      </a>
    </div>
  </div>
  <h2>Other Idols</h2>
  <div class="newholder">
    <div class="newfeature">
      <div class="otherstory-title">
        <a href="/2050/05/25/a-story-thats-mine-alone/"><b>Mika FS2</b></a>
      </div>
      <a href="/2050/05/25/a-story-thats-mine-alone/">
        <img src="https://res.cloudinary.com/djq41tb84/image/upload/v1714780298/translation%20site/masterlist/ny3rpxgmxlzeri6ppcbs.png" alt="story img"></a>
    </div>
    <div class="newfeature">
      <div class="otherstory-title">
        <a href="/2050/07/05/esu-idolstory-1/"><b>Esu Idol Story 1</b></a>
      </div>
      <a href="/2050/07/05/esu-idolstory-1/">
        <img src="https://res.cloudinary.com/djq41tb84/image/upload/v1715052275/translation%20site/masterlist/dmiderxybuyssfwlhu0n.png" alt="story img"></a>
    </div>
  </div>
  <h2>Song Translations</h2>
  <sup><i>If you’d like to use my song translations for edits, you’re welcome to do so as long as there is <b>clear, visible credit</b> either in the video or in the description.</i></sup>
  <div id="songs">
    <div class="song-item">
      <figure class="song-figure">
        <a href="/2023/05/22/turbulent-storm/" class="song-caption">
          <figcaption>
            <h4>Turbulent Storm</h4>
          </figcaption>
        </a>
        <img src="https://res.cloudinary.com/djq41tb84/image/upload/v1709337756/translation%20site/cyeuwjz9rfdp4t6gnmcn.png" class="song-image rotate" />
      </figure>
    </div>
    <div class="song-item">
      <figure class="song-figure">
        <a href="/2023/05/30/trip-album/" class="song-caption">
          <figcaption>
            <h4>TRIP</h4>
              <p>Crazy:B</p>
          </figcaption>
        </a>
        <img src="https://res.cloudinary.com/djq41tb84/image/upload/v1709337910/translation%20site/sfqfdn4fdj4u9l76vcby.png" class="song-image rotate" />
      </figure>
    </div>
    <!--- more songs go here --->
  </div>
  <div>
  </div>
  <!--- aaaa --->
  <!-- more translation categories can go here -->
</main>
<div>
<!-- add sections above this point -->
<!--- 
story template looks like this:
      <div class="story">
      <div class="image">
        <img src="[UNBL-URL]" alt="[STORY NAME]">
      </div>
      <a href="[STORY URL]" class="storyName" target="_blank">
        <span>Example</span> 
        <span class="read">
        </span>
      </a>
      </div>
    </div>
    --->
</div>
</div>
