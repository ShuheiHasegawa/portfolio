<template>
  <div id="smooth-wrapper">
    <div id="smooth-content">
      <div class="layout-container relative">
        <Opening/>
        <LazyHeader/>
        <!--      <Banner/>-->
        <LazyPanels/>
        <LazyFooter/>
      </div>
    </div>
  </div>
</template>

<script>
import gsap from "gsap";

import {Draggable} from "gsap/Draggable";
// gsap.registerPlugin(Draggable);

import {InertiaPlugin} from "gsap-trial/InertiaPlugin";
// gsap.registerPlugin(InertiaPlugin);

import {ScrollTrigger} from "gsap/ScrollTrigger";
// gsap.registerPlugin(ScrollTrigger);

import {ScrollSmoother} from 'gsap-trial/ScrollSmoother';
// gsap.registerPlugin(ScrollSmoother);

if (process.client) {
  gsap.registerPlugin(Draggable, InertiaPlugin, ScrollTrigger, ScrollSmoother);
}

// ScrollSmoother.create({
//   smooth: 1,               // how long (in seconds) it takes to "catch up" to the native scroll position
  // effects: true,           // looks for data-speed and data-lag attributes on elements
  // smoothTouch: 0.1,        // much shorter smoothing time on touch devices (default is NO smoothing on touch devices)
// });

</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Kiwi+Maru&family=Roboto:wght@300&display=swap');

body {
  height: 100vh;
  width: 100vw;
  font-family: 'Kiwi Maru', serif;
  background-color: #fff;
  color: rgba(0, 0, 0, 0.8);
  overflow: hidden;
}

.layout-container {
  width: 100vw;
  overflow: hidden;
}

.dark-mode body {
  background-color: #091a28;
  color: #ebf4f1;
}

.sepia-mode body {
  background-color: #f1e7d0;
  color: #433422;
}

.color-one-mode body {
  background-color: #F4EEE7;
  color: #433422;
}

.color-two-mode body {
  background-color: #FFAA73;
  color: #433422;
}

.color-three-mode body {
  background-color: #EFE7DF;
  color: #433422;
}

.color-four-mode body {
  background-color: #C1E1E9;
  color: #433422;
}

.color-five-mode body {
  background-color: #FF849E;
  color: #433422;
}

.color-six-mode body {
  background-color: #846A6A;
  color: #433422;
}

.color-seven-mode body {
  background-color: #E0ABF2;
  color: #433422;
}

.color-eight-mode body {
  background-color: #C7E5D5;
  color: #433422;
}

.light-theme {
  background-color: #fff;
}

.dark-theme {
  background-color: #091a28;
}

.sepia-theme {
  background-color: #f1e7d0;
}

.color-one-theme {
  background-color: #F4EEE7;
}

.color-two-theme {
  background-color: #FFAA73;
}

.color-three-theme {
  background-color: #EFE7DF;
}

.color-four-theme {
  background-color: #C1E1E9;
}

.color-five-theme {
  background-color: #FF849E;
}

.color-six-theme {
  background-color: #846A6A;
}

.color-seven-theme {
  background-color: #E0ABF2;
}

.color-eight-theme {
  background-color: #C7E5D5;
}

.color-one {
  background-color: #F4EEE7;
  height: 20vh;
}
.color-two {
  background-color: #FFAA73;
  /*height: 20vh;*/
}
.color-three {
  background-color: #EFE7DF;
  height: 20vh;
}
.color-four {
  background-color: #C1E1E9;
  height: 20vh;
}
.color-five {
  background-color: #FF849E;
  height: 20vh;
}
.color-six {
  background-color: #846A6A;
  height: 20vh;
}
.color-seven {
  background-color: #E0ABF2;
  height: 20vh;
}
.color-eight {
  background-color: #C7E5D5;
  height: 20vh;
}
</style>