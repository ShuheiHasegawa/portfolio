<template>
  <div id="circle03" class="bg-circle-container">
    <div class="bg-circle bg-circle-03"></div>
    <div class="bg-circle-back color-two"></div>
  </div>
  <div id="circle04" class="bg-circle-container">
    <div class="bg-circle bg-circle-04"></div>
    <div class="bg-circle-back color-three"></div>
  </div>
  <div id="circle05" class="bg-circle-container">
    <div class="bg-circle bg-circle-05"></div>
    <div class="bg-circle-back color-four"></div>
  </div>
  <div id="circle06" class="bg-circle-container">
    <div class="bg-circle bg-circle-06"></div>
    <div class="bg-circle-back color-six"></div>
  </div>
  <div id="circle07" class="bg-circle-container">
    <div class="bg-circle bg-circle-07"></div>
    <div class="bg-circle-back color-seven"></div>
  </div>
  <div id="circle08" class="bg-circle-container">
    <div class="bg-circle bg-circle-08"></div>
    <div class="bg-circle-back color-eight"></div>
  </div>
  <div id="circle09" class="bg-circle-container">
    <div class="bg-circle bg-circle-09"></div>
    <div class="bg-circle-back color-nine"></div>
  </div>

  <div class="second">
    <div class="text-center my-8" style="display: none;">
      <transition
          appear
          @before-enter="beforePhoto"
          @enter="enterPhoto"
          @after-enter="afterPhoto"
      >
        <nuxt-img
            src="/yuka/vertical/17.webp"
            format="webp"
            loading="lazy"
        />
      </transition>
    </div>

<!--    <div class="grid grid-cols-3 pt-48 gap-16 photo-row1">-->
<!--      <div class="md:col-span-1 col-span-3">-->
<!--        <img src="@/assets/photos/_DSC0871.webp" alt="" height="600">-->
<!--      </div>-->
<!--      <div class="md:col-span-1 col-span-3">-->
<!--        <img src="@/assets/photos/_DSC1146.webp" alt="" height="600">-->
<!--      </div>-->
<!--      <div class="md:col-span-1 col-span-3">-->
<!--        <img src="@/assets/photos/_DSC0890.webp" alt="" height="600">-->
<!--      </div>-->
<!--    </div>-->

<!--    <swiper-->
<!--        :effect="'coverflow'"-->
<!--        :grabCursor="true"-->
<!--        :centeredSlides="true"-->
<!--        :slidesPerView="'auto'"-->
<!--        :coverflowEffect="{-->
<!--            rotate: 50,-->
<!--            stretch: 0,-->
<!--            depth: 100,-->
<!--            modifier: 1,-->
<!--            slideShadows: true,-->
<!--          }"-->
<!--        :pagination="true"-->
<!--        :modules="modules"-->
<!--        class="mySwiper"-->
<!--        style="display: none;"-->
<!--    >-->
<!--      <swiper-slide-->
<!--      ><img-->
<!--          src="https://swiperjs.com/demos/images/nature-1.webp"/></swiper-slide-->
<!--      >-->
<!--      <swiper-slide-->
<!--      ><img-->
<!--          src="https://swiperjs.com/demos/images/nature-2.webp"/></swiper-slide-->
<!--      >-->
<!--      <swiper-slide-->
<!--      ><img-->
<!--          src="https://swiperjs.com/demos/images/nature-3.webp"/></swiper-slide-->
<!--      >-->
<!--      <swiper-slide-->
<!--      ><img-->
<!--          src="https://swiperjs.com/demos/images/nature-4.webp"/></swiper-slide-->
<!--      >-->
<!--      <swiper-slide-->
<!--      ><img-->
<!--          src="https://swiperjs.com/demos/images/nature-5.webp"/></swiper-slide-->
<!--      >-->
<!--      <swiper-slide-->
<!--      ><img-->
<!--          src="https://swiperjs.com/demos/images/nature-6.webp"/></swiper-slide-->
<!--      >-->
<!--      <swiper-slide-->
<!--      ><img-->
<!--          src="https://swiperjs.com/demos/images/nature-7.webp"/></swiper-slide-->
<!--      >-->
<!--      <swiper-slide-->
<!--      ><img-->
<!--          src="https://swiperjs.com/demos/images/nature-8.webp"/></swiper-slide-->
<!--      >-->
<!--      <swiper-slide-->
<!--      ><img src="https://swiperjs.com/demos/images/nature-9.webp"-->
<!--      /></swiper-slide>-->
<!--    </swiper>-->

    <div class="relative my-32">
      <div>
        <img class="gray-circle01 bg-gray-600 opacity-50"/>
      </div>
      <div class="mt-16">
        <img class="gray-circle02 bg-gray-600 opacity-50"/>
      </div>
      <div class="mt-16">
        <img class="gray-circle03 bg-gray-600 opacity-50"/>
      </div>
    </div>

<!--    <SideScrollingPanel/>-->

    <ScrollingPanel/>

<!--    <div class="panel4 bg-white">-->
<!--      <h2 class="text-base text1">Everything you need</h2>-->
<!--    </div>-->

    <div class="polaroid-container h-screen w-screen flex justify-center items-center my-32">
      <ul id="polaroids">
        <li><a href="#polaroids" title="????????????">
          <nuxt-img
              src="/yuka/vertical/16.webp"
              format="webp"
              loading="lazy"
          />
        </a></li>
        <li><a href="#polaroids" title="?????????">
          <nuxt-img
              src="/yuka/vertical/10.webp"
              format="webp"
              loading="lazy"
          />
        </a></li>
        <li><a href="#polaroids" title="?????????">
          <nuxt-img
              src="/yuka/vertical/36.webp"
              format="webp"
              loading="lazy"
          />
        </a></li>
        <li><a href="#polaroids" title="?????????">
          <nuxt-img
              src="/yuka/vertical/52.webp"
              format="webp"
              loading="lazy"
          />
        </a></li>
        <li><a href="#polaroids" title="??????????????????">
          <nuxt-img
              src="/yuka/vertical/134.webp"
              format="webp"
              loading="lazy"
          />
        </a></li>
        <li><a href="#polaroids" title="?????????????????????">
          <nuxt-img
              src="/yuka/vertical/125.webp"
              format="webp"
              loading="lazy"
          />
        </a></li>
      </ul>
    </div>
  </div>

</template>

<script>
import gsap from "gsap"
// import {Swiper, SwiperSlide} from "swiper/vue"
// import {EffectCoverflow, Pagination} from "swiper"
// import "swiper/swiper-bundle.css"

export default {
  components: {
    // Swiper,
    // SwiperSlide,
  },
  mounted() {
    this.scrollAnimation()
  },
  methods: {
    scrollAnimation() {
      // gsap.timeline({
      //   scrollTrigger: {
      //     trigger: ".box",
      //     start: "center center",
      //     end: "bottom top",
      //     // markers: true,
      //     scrub: true,
      //     pin: true,
      //   }
      // })
      //     .from(".text1", {x: innerWidth * 1, opacity: 0, duration: 5})

      // gsap.timeline({
      //   scrollTrigger: {
      //     trigger: ".box2",
      //     start: "center center",
      //     end: "bottom top",
      //     // markers: true,
      //     scrub: true,
      //     pin: true,
      //   }
      // })
      //     .from(".text4", {x: innerWidth * 1, opacity: 0})
      //     .from(".text5", {x: innerWidth * 1, opacity: 0})

      // gsap
      //     .timeline({
      //       defaults: {ease: "power2.out", duration: 1}, // timeline??????????????????
      //       scrollTrigger: {
      //         // markers: true, // ?????????????????????????????????????????????
      //         trigger: ".photo-row1", // ???????????????????????????????????????????????????
      //         start: "top 50%", // ???????????????????????????????????????????????????????????????
      //         end: "bottom top", // ?????????????????????????????????????????????????????????????????????
      //         toggleActions: "restart none none none", // ?????????????????????????????????????????????????????????????????????
      //       },
      //     })
      //     .from(".photo-row2", {
      //       delay: 0.5,
      //       duration: 0.5,
      //       opacity: 0,
      //       x: 100,
      //     })
      //     .to(".photo-row2", {
      //       duration: 0.5,
      //       opacity: 1,
      //     })
      //     .from(".photo-row3", {
      //       delay: 0.5,
      //       duration: 0.5,
      //       opacity: 0,
      //       x: -100,
      //     })
      //     .to(".photo-row3", {
      //       duration: 0.5,
      //       opacity: 1,
      //     })

      // ??????????????????
      const wrapper = document.querySelector('#wrapper');
      if(wrapper) {
        // gsap.registerPlugin(ScrollTrigger); // npm/yarn???????????????
        const panels = gsap.utils.toArray('.panel');
        const wrapperWidth = wrapper.offsetWidth;
        /**
         * ????????????????????????
         */
        gsap.to( panels, {
          xPercent: -100 * (panels.length - 1), // transformX
          ease: "none", // easing?????????
          scrollTrigger: { // scrollTrigger
            trigger: wrapper, // ?????????????????????????????????????????????
            pin: true, // ?????????????????????
            scrub: 1, // ???????????????????????????????????????????????????????????????????????????????????????
            snap: { // ????????????????????????????????????
              snapTo: 1 / ( panels.length - 1 ), // ????????????????????????????????????
              duration: {min: .4, max: .6}, // ?????????????????????????????????????????????
              ease: "none" // easing
            },
            end: () => "+=" + wrapperWidth // ?????????????????????????????????????????????
          }
        })
      }

      gsap
          .timeline({
            defaults: {
              ease: "power2.out", duration: 1
            }, // timeline??????????????????
            scrollTrigger: {
              // markers: true, // ?????????????????????????????????????????????
              trigger: "#circle03", // ???????????????????????????????????????????????????
              start: "center bottom", // ???????????????????????????????????????????????????????????????
              end: "top top", // ?????????????????????????????????????????????????????????????????????
              // start: 'top bottom',
              // end: 'bottom top',
              // toggleActions: "restart none none none", // ?????????????????????????????????????????????????????????????????????
              toggleActions: "play reverse play reverse", // ?????????????????????????????????????????????????????????????????????
              scrub: true, // ????????????????????????????????????
              // pin: true,
              // onScrubComplete: self => {
              // if(self.progress === 1) {
              //   self.kill();
              //   self.set(".bg-circle-01, .bg-circle-02", {
              //     scale: 0,
              //   })
              // }
              // }
            },
          })
          .from("#circle03 > .bg-circle, #circle03 > .bg-circle-back", {
            delay: 0.5,
            duration: 0.5,
            opacity: 1,
            scale: 0.1,
            y: '200%',
          })
          .to("#circle03 > .bg-circle", {
            // x: '100%',
            opacity: 0,
            duration: 0.5,
            scale: 3.0,
          })
          .to("#circle03 > .bg-circle-back", {
            // x: '100%',
            duration: 0.5,
            scale: 3.0,
          }, "<")

      gsap
          .timeline({
            defaults: {
              ease: "power2.out", duration: 1
            }, // timeline??????????????????
            scrollTrigger: {
              // markers: true, // ?????????????????????????????????????????????
              trigger: "#circle04", // ???????????????????????????????????????????????????
              start: "center bottom", // ???????????????????????????????????????????????????????????????
              end: "top top", // ?????????????????????????????????????????????????????????????????????
              // start: 'top bottom',
              // end: 'bottom top',
              // toggleActions: "restart none none none", // ?????????????????????????????????????????????????????????????????????
              toggleActions: "play reverse play reverse", // ?????????????????????????????????????????????????????????????????????
              scrub: true, // ????????????????????????????????????
              // onScrubComplete: self => {
              // if(self.progress === 1) {
              //   self.kill();
              //   self.set(".bg-circle-01, .bg-circle-02", {
              //     scale: 0,
              //   })
              // }
              // }
            },
          })
          .from("#circle04 > .bg-circle, #circle04 > .bg-circle-back", {
            delay: 0.5,
            duration: 0.5,
            opacity: 1,
            scale: 0.1,
            y: '200%',
          })
          .to("#circle04 > .bg-circle", {
            // x: '100%',
            opacity: 0,
            duration: 0.5,
            scale: 3.0,
          })
          .to("#circle04 > .bg-circle-back", {
            // x: '100%',
            duration: 0.5,
            scale: 3.0,
          }, "<")

      gsap
          .timeline({
            defaults: {
              ease: "power2.out", duration: 1
            },
            scrollTrigger: {
              trigger: "#circle05", // ???????????????????????????????????????????????????
              start: "center bottom", // ???????????????????????????????????????????????????????????????
              end: "top top", // ?????????????????????????????????????????????????????????????????????
              toggleActions: "play reverse play reverse", // ?????????????????????????????????????????????????????????????????????
              scrub: true, // ????????????????????????????????????
            },
          })
          .from("#circle05 > .bg-circle, #circle05 > .bg-circle-back", {
            delay: 0.5,
            duration: 0.5,
            opacity: 1,
            scale: 0.1,
            y: '200%',
          })
          .to("#circle05 > .bg-circle", {
            // x: '100%',
            opacity: 0,
            duration: 0.5,
            scale: 3.0,
          })
          .to("#circle05 > .bg-circle-back", {
            duration: 0.5,
            scale: 3.0,
          }, "<")

      gsap
          .timeline({
            defaults: {
              ease: "power2.out", duration: 1
            },
            scrollTrigger: {
              trigger: "#circle06", // ???????????????????????????????????????????????????
              start: "center bottom", // ???????????????????????????????????????????????????????????????
              end: "top top", // ?????????????????????????????????????????????????????????????????????
              toggleActions: "play reverse play reverse", // ?????????????????????????????????????????????????????????????????????
              scrub: true, // ????????????????????????????????????
            },
          })
          .from("#circle06 > .bg-circle, #circle06 > .bg-circle-back", {
            delay: 0.5,
            duration: 0.5,
            opacity: 1,
            scale: 0.1,
            y: '200%',
          })
          .to("#circle06 > .bg-circle", {
            // x: '100%',
            opacity: 0,
            duration: 0.5,
            scale: 3.0,
          })
          .to("#circle06 > .bg-circle-back", {
            duration: 0.5,
            scale: 3.0,
          }, "<")

      gsap
          .timeline({
            defaults: {
              ease: "power2.out", duration: 1
            },
            scrollTrigger: {
              trigger: "#circle07", // ???????????????????????????????????????????????????
              start: "center bottom", // ???????????????????????????????????????????????????????????????
              end: "top top", // ?????????????????????????????????????????????????????????????????????
              toggleActions: "play reverse play reverse", // ?????????????????????????????????????????????????????????????????????
              scrub: true, // ????????????????????????????????????
            },
          })
          .from("#circle07 > .bg-circle, #circle07 > .bg-circle-back", {
            delay: 0.5,
            duration: 0.5,
            opacity: 1,
            scale: 0.1,
            y: '200%',
          })
          .to("#circle07 > .bg-circle", {
            // x: '100%',
            opacity: 0,
            duration: 0.5,
            scale: 3.0,
          })
          .to("#circle07 > .bg-circle-back", {
            duration: 0.5,
            scale: 3.0,
          }, "<")

      gsap
          .timeline({
            defaults: {
              ease: "power2.out", duration: 1
            },
            scrollTrigger: {
              trigger: "#circle08", // ???????????????????????????????????????????????????
              start: "center bottom", // ???????????????????????????????????????????????????????????????
              end: "top top", // ?????????????????????????????????????????????????????????????????????
              toggleActions: "play reverse play reverse", // ?????????????????????????????????????????????????????????????????????
              scrub: true, // ????????????????????????????????????
            },
          })
          .from("#circle08 > .bg-circle, #circle08 > .bg-circle-back", {
            delay: 0.5,
            duration: 0.5,
            opacity: 1,
            scale: 0.1,
            y: '200%',
          })
          .to("#circle08 > .bg-circle", {
            // x: '100%',
            opacity: 0,
            duration: 0.5,
            scale: 3.0,
          })
          .to("#circle08 > .bg-circle-back", {
            duration: 0.5,
            scale: 3.0,
          }, "<")

      gsap
          .timeline({
            defaults: {
              ease: "power2.out", duration: 1
            },
            scrollTrigger: {
              trigger: "#circle09", // ???????????????????????????????????????????????????
              start: "center bottom", // ???????????????????????????????????????????????????????????????
              end: "top top", // ?????????????????????????????????????????????????????????????????????
              toggleActions: "play reverse play reverse", // ?????????????????????????????????????????????????????????????????????
              scrub: true, // ????????????????????????????????????
            },
          })
          .from("#circle09 > .bg-circle, #circle09 > .bg-circle-back", {
            delay: 0.5,
            duration: 0.5,
            opacity: 1,
            scale: 0.1,
            y: '200%',
          })
          .to("#circle09 > .bg-circle", {
            // x: '100%',
            opacity: 0,
            duration: 0.5,
            scale: 3.0,
          })
          .to("#circle09 > .bg-circle-back", {
            duration: 0.5,
            scale: 3.0,
          }, "<")



    }, // scrollAnimation

  },
  setup() {
    const photoList1 = [
      {path: "/photos/_DSC1146.webp"},
      {path: "/photos/_DSC1146.webp"},
      {path: "/photos/_DSC1146.webp"},
    ]
    const photoList2 = [
      {path: "/photos/_DSC1146.webp"},
      {path: "/photos/_DSC1146.webp"},
      {path: "/photos/_DSC1146.webp"},
    ]
    const photoList3 = [
      {path: "/photos/_DSC1146.webp"},
      {path: "/photos/_DSC1146.webp"},
      {path: "/photos/_DSC1146.webp"},
    ]

    // ??????????????????????????????????????????????????????
    // ?????????????????????????????????
    const panelsBeforeEnter = (el) => {
      gsap.set(el, {
        y: 100,
        opacity: 0
      })
    }
    // ??????????????????????????????????????????
    const panelsEnter = (el, done) => {
      gsap.to(el, {
        opacity: 1,
        y: 0,
        duration: 0.8,
        delay: 1 + el.dataset.index * 0.2,
        onComplete: done
      })
    }

    const enter = (el, done) => {
      gsap.to(el, {
        scrollTrigger: {
          trigger: el,
          toggleActions: "restart none none none"
        },
        duration: 3,
        y: 0,
        opacity: 1,
        ease: "expo.out",
        onComplete: done
      })
    }

    const beforePhoto = (el, done) => {
      gsap.to(el, {
        y: 0,
        scrollTrigger: {
          trigger: el,
          start: 'top bottom',
          end: 'bottom top',
          scrub: 0.5
          //markers: true
        }
      });
    }

    const enterPhoto = (el, done) => {
      gsap.to(el, {
        y: 100,
        scrollTrigger: {
          trigger: el,
          start: 'top bottom',
          end: 'bottom top',
          scrub: 0.5
          //markers: true
        }
      });
    }

    const afterPhoto = (el, done) => {
      gsap.to(el, {
        y: 500,
        scrollTrigger: {
          trigger: el,
          start: 'top bottom',
          end: 'bottom top',
          scrub: 0.5
          //markers: true
        }
      });
    }

    // const onSwiper = (swiper) => {
    //   console.log(swiper)
    // }
    // const onSlideChange = () => {
    //   console.log("slide change")
    // }

    return {
      // onSwiper,
      // onSlideChange,
      panelsBeforeEnter,
      panelsEnter,
      enter,
      beforePhoto,
      enterPhoto,
      afterPhoto,
      // modules: [EffectCoverflow, Pagination],
      photoList1,
      photoList2,
      photoList3,
    }
  }
}
</script>

<style scoped>
.swiper {
  width: 100%;
  padding-top: 50px;
  padding-bottom: 50px;
}

.swiper-slide {
  background-position: center;
  background-size: cover;
  width: 300px;
  height: 300px;
}

.swiper-slide img {
  display: block;
  width: 100%;
}

.gray-circle01 {
  width: 60vw;
  height: 60vw;
  background-image: url("@/assets/photos/yuka/horizontal/5.webp");
  background-size: cover;
  background-position: right 30% top 20px;
  border-radius: 50%;
  margin: 0 auto;
  pointer-events: none;
}
.gray-circle02 {
  width: 60vw;
  height: 60vw;
  background-image: url("@/assets/photos/yuka/vertical/12.webp");
  background-size: cover;
  border-radius: 50%;
  margin: 0 auto;
  pointer-events: none;
}
.gray-circle03 {
  width: 60vw;
  height: 60vw;
  background-image: url("@/assets/photos/yuka/horizontal/14.webp");
  background-size: cover;
  border-radius: 50%;
  margin: 0 auto;
  pointer-events: none;
}

.polaroid-container {
  height: 100%;
  /*height: 250vmax;*/
}
/*@media (min-width: 480px) {*/
/*  .panel5 {*/
/*    height: 75vh;*/
/*  }*/
/*}*/

@font-face {
  font-family: 'Hina2ndGrade';
  src: url('@/assets/font/Hina2ndGrade.woff');
}

ul#polaroids {
  list-style-type: none;
  width: 30vmax;
}

ul#polaroids li a {
  position: relative;
  float: left;
  padding: 10px 10px 20px;
  background-color: white;

  -moz-box-shadow: 0 4px 10px #333;
  -webkit-box-shadow: 0 4px 10px #333;
  box-shadow: 0 4px 10px #333;

  -webkit-transform: rotate(5deg);
  -moz-transform: rotate(5deg);
  transform: rotate(5deg);

  width: 30vmax;
  /*width: 200px;*/
  text-decoration: none;
  text-align: center;
}
ul#polaroids li:nth-child(2n+1) a {
  -webkit-transform: rotate(-10deg);
  -moz-transform: rotate(-10deg);
  transform: rotate(-10deg);
  position: relative;
  top: -5px;
}
ul#polaroids li:nth-child(3) a {
  -webkit-transform: rotate(30deg);
  -moz-transform: rotate(30deg);
  transform: rotate(30deg);
  position: relative;
  top: -10px;
  left: 30px;
}
ul#polaroids li:nth-child(4) a {
  position: relative;
  top: -10px;
  left: 10px;
}
ul#polaroids li a img {
  width: 30vmax;
  /*height: 200px;*/
  margin-bottom: 10px;
  background-size: cover;
}
ul#polaroids a:after {
  content: attr(title);
  font-family: 'Hina2ndGrade', sans-serif;
  color: #333;
}

ul#polaroids li a:hover {
  -webkit-transform: scale(1.25);
  -moz-transform: scale(1.25);
  transform: scale(1.25);
  z-index: 6;
}

.bg-circle-container {
  height: 100%;
  width: 100vw;
  position: relative;
}
.bg-circle {
  border-radius: 50%;
  height: 50vmax;
  margin: 0 auto;
  pointer-events: none;
  right: -6vw;
  top: 5vh;
  width: 50vmax;
  z-index: -1;
}
.bg-circle-03 {
  background-image: url("@/assets/photos/yuka/vertical/2.webp");
  background-size: cover;
}
.bg-circle-04 {
  background-image: url("@/assets/photos/yuka/horizontal/11.webp");
  background-size: cover;
}
.bg-circle-05 {
  background-image: url("@/assets/photos/yuka/vertical/14.webp");
  background-size: cover;
}
.bg-circle-06 {
  background-image: url("@/assets/photos/yuka/vertical/26.webp");
  background-size: cover;
}
.bg-circle-07 {
  background-image: url("@/assets/photos/yuka/vertical/47.webp");
  background-size: cover;
}
.bg-circle-08 {
  background-image: url("@/assets/photos/yuka/vertical/82.webp");
  background-size: cover;
}
.bg-circle-09 {
  background-image: url("@/assets/photos/yuka/horizontal/48.webp");
  background-size: cover;
}
.bg-circle-back {
  border-radius: 50%;
  height: 50vmax;
  left: 50%;
  pointer-events: none;
  position: absolute;
  top: 50%;
  width: 50vmax;
  transform: translate(-50%, -50%);
  z-index: -1;
}

</style>