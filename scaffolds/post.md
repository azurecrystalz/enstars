---
title: { { title } }
date: { { date } }
categories:
tags:
description:
---

<div class="preview-wrapper reverse" style="--storyColor: #hex;--storyColor-rgb: r,g,b;--storyColor-h: hue;--storyColor-s: saturation%;--storyColor-l: lightness%;">
  <div class="grid-wrapper">
      <div class="preview-background" style="background-image: url('[BLOOMED_CARD_URL]')"></div>
      <div class="preview-box" style="background: calc(var(--card-background) + 2%)">
          <div class="title-area">
              <div class="title-area__title"><!-- STORY ENG TITLE --></div>
              <div class="title-area__subtitle"><!-- STORY JP TITLE --> </div>
              <div class="title-area__start"><a href="[STORY_LINK_GOES_HERE]">Start Reading</a></div>
          </div>
          <div class="info-area">
              <div class="synopsis" style="width: 90%;">
                <!-- SYNOPSIS GOES HERE -->
              </div>
              <div class="info">
                  <div class="info-item season">
                      <div class="label">
                          Season
                      </div>
                      <div class="value">
                        <!-- STORY SEASON -->
                      </div>
                  </div>
                  <div class="info-item chapters">
                      <div class="label">
                          Chapters
                      </div>
                      <div class="value">
                          <!-- NUMBER OF CHAPTERS -->
                      </div>
                  </div>
                  <div class="info-item characters">
                      <div class="label">
                          Characters
                      </div>
                      <div class="value">
                        <!-- 
                          <a href="/tags/[CHARACTER_LAST_NAME]-[CHARACTER_FIRST_NAME]/" character="[CHARACTER_FIRST_AME]" title="[CHARACTER_FIRST_NAME]"></a>
                         -->
                         <!-- COPY AND PASTE THE ABOVE FOR EACH CHARACTER THAT APPEARS IN THE STORY -->
                      </div>
                  </div>
                  <div class="info-item tl">
                      <div class="label">
                          Translator
                      </div>
                      <div class="value">
                          <a href="https://twitter.com/azurecrystalz">aurora</a>
                      </div>
                  </div>
                  <div class="info-item pr">
                      <div class="label">
                          Proofreaders
                      </div>
                      <div class="value">
                        <a href="https://tumblr.com/starswallowingsea">shay</a> or <a href="https://tumblr.com/pitxroxas">pit</a>
                          <!-- PROOFREADER LIST (IF ANY) -->
                      </div>
                  </div>
              </div>
          </div>
      </div>
  </div>
</div>

<!-- more -->

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
    .hint--error:after {
      background-color: #374A5D;
      text-shadow: 0 -1px 0px #23384C;
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
    [character="Anzu"] {
      --color: #ffb6da;
      --hue: 330.4;
      --name: "Anzu";
      --charahead: url("https://cdn.jsdelivr.net/gh/toujokaname/images@main/icons/anzu_charahead.png");
  }    
  </style>

  <!-- CONTENT GOES HERE -->

  <!-- 
  SPEECH BUBBLE FORMAT: 
  {% bubble [CHARACTER_FIRST_NAME] [ATTRIBUTE(optional)]}
    DIALOGUE TEXT HERE

    ADD A LINE SPACE FOR A NEW LINE

    <th>EMBED THOUGHT DIALOGUE WITH THESE TAGS</th>
  {% endbubble %}
  -->

  </div>
