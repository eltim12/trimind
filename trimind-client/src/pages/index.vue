<template>
  <!-- <div class="home-page" id="home-page" data-scroll-container> -->
  <div class="home-page" id="home-page">
    <section class="banner-section">
      <GradientBackgroundLeft />
      <GradientBackgroundRight />
      <div
        class="banner-content d-flex flex-column align-center justify-center"
        ref="scrollContainer"
      >
        <img src="@/assets/logo.svg" alt="" width="200px" />
        <div class="text my-10">
          <!-- <div
            class="heading text-mono"
            data-scroll
            data-scroll-direction="veritcal"
            data-scroll-speed="3"
          >
            Crafting Digital Experiences <br />
            Beyond Imaginations
          </div> -->

          <div class="heading text-mono">
            Crafting Digital Experiences <br />
            Beyond Imaginations
          </div>
          <div class="subheading mt-5" data-scroll>
            Combining reativity with technical expertise to deliver tailor-made
            solutions that meet our clients' unique needs.
          </div>
        </div>
        <TrimindButton :text="'Start a project'" data-scroll />
      </div>
      <div class="field-section d-flex flex-column">
        <div class="description-wrapper d-flex flex-row justify-space-between">
          <v-row>
            <v-col cols="3">
              <img
                src="@/assets/logo-icon.svg"
                alt=""
                width="50px"
                data-scroll
              />
            </v-col>
            <v-col cols="9">
              <div class="description" data-scroll>
                At TriMind Studio, our diverse and innovative team is dedicated
                to exceeding client expectations with exceptional results.
              </div>
              <div class="fields-content mt-16" data-scroll>
                <v-row>
                  <v-col cols="12" class="mb-7"> Our Services </v-col>
                  <v-col cols="6">
                    <small class="mr-7"> 01 </small>
                    Custom Web Development
                  </v-col>
                  <v-col cols="6">
                    <small class="mr-7"> 02 </small>
                    App Design & Development
                  </v-col>
                  <v-col cols="6">
                    <small class="mr-7"> 03 </small>
                    UI / UX Design
                  </v-col>
                  <v-col cols="6">
                    <small class="mr-7"> 04 </small>
                    E-Commerce Solutions
                  </v-col>
                  <v-col cols="6">
                    <small class="mr-7"> 05 </small>
                    Software Consulting
                  </v-col>
                  <v-col cols="6">
                    <small class="mr-7"> 06 </small>
                    AI Automation Solutions
                  </v-col>
                </v-row>
              </div>
            </v-col>
          </v-row>
        </div>
      </div>

      <div
        class="approach-section d-flex flex-column justify-center align-center"
      >
        <GradientBackgroundRight />
        <!-- <GradientBackgroundLeft /> -->
        <div class="approach-content">
          <v-row>
            <v-col cols="12">
              <div class="heading text-mono mb-3">Approach</div>
            </v-col>
            <v-col cols="12">
              <v-row>
                <v-col cols="6">
                  <img
                    src="@/assets/approach-page/consulting-icon.svg"
                    alt=""
                    width="30px"
                  />
                  <div class="subheading my-3">Consulting</div>
                  <div class="text">
                    To better understand your goals, design preferences, and
                    target audience, we'll be asking you a series of questions.
                    This initial step is crucial in establishing a strong
                    foundation for our collaboration.
                  </div>
                </v-col>
                <v-col cols="6">
                  <img
                    src="@/assets/approach-page/collaborative-icon.svg"
                    alt=""
                    width="30px"
                  />
                  <div class="subheading my-3">Colaborative Review</div>
                  <div class="text">
                    During the design phase, we invite our clients to review and
                    provide feedback. This collaborative approach ensures
                    optimal structure and functionality from the outset.
                  </div>
                </v-col>
                <v-col cols="6">
                  <img
                    src="@/assets/approach-page/iterate-icon.svg"
                    alt=""
                    width="30px"
                  />
                  <div class="subheading my-3">Iterate</div>
                  <div class="text">
                    Polishing and attention to details are important when it
                    comes to the final product. We're iterating until you're
                    happy with the results.
                  </div>
                </v-col>
                <v-col cols="6">
                  <img
                    src="@/assets/approach-page/make-it-icon.svg"
                    alt=""
                    width="30px"
                  />
                  <div class="subheading my-3">Make it pop</div>
                  <div class="text">
                    We establish a structure focused on functionality and
                    accessibility, incorporating interactions and animations
                    that ensure complete immersion.
                  </div>
                </v-col>
              </v-row>
            </v-col>
            <!-- <v-cols cols="3" class="d-flex align-center">
              <TrimindButton :text="'Let\'s work together'" :large="true"/>
            </v-cols> -->
          </v-row>
        </div>
      </div>

      <div class="field-section d-flex flex-column">
        <div class="description-wrapper d-flex flex-row justify-space-between">
          <v-row>
            <v-col cols="3">
              <img src="@/assets/logo-icon.svg" alt="" width="50px" />
            </v-col>
            <v-col cols="9">
              <div class="description">
                At TriMind Studio, our diverse and innovative team is dedicated
                to exceeding client expectations with exceptional results.
              </div>
              <div class="fields-content mt-16">
                <v-row>
                  <v-col cols="12" class="mb-7"> Our Services </v-col>
                  <v-col cols="6">
                    <small class="mr-7"> 01 </small>
                    Custom Web Development
                  </v-col>
                  <v-col cols="6">
                    <small class="mr-7"> 02 </small>
                    App Design & Development
                  </v-col>
                  <v-col cols="6">
                    <small class="mr-7"> 03 </small>
                    UI / UX Design
                  </v-col>
                  <v-col cols="6">
                    <small class="mr-7"> 04 </small>
                    E-Commerce Solutions
                  </v-col>
                  <v-col cols="6">
                    <small class="mr-7"> 05 </small>
                    Software Consulting
                  </v-col>
                  <v-col cols="6">
                    <small class="mr-7"> 06 </small>
                    AI Automation Solutions
                  </v-col>
                </v-row>
              </div>
            </v-col>
          </v-row>
        </div>
      </div>

      <div class="title-section d-flex flex-column justify-center align-center">
        <GradientBackgroundRight />
        <GradientBackgroundLeft />
        <div class="text mb-6">
          <div class="heading">Our Masterpiece</div>
        </div>
        <TrimindButton :text="'Check it out'" />
      </div>

      <div class="project-section d-flex flex-column">
        <div class="description-wrapper d-flex flex-row justify-space-between">
          <v-row>
            <v-col cols="3">
              <img src="@/assets/logo-icon.svg" alt="" width="50px" />
            </v-col>
            <v-col cols="9">
              <div class="description">
                At TriMind, we merge creativity and technology to craft digital
                solutions that inspire and engage. With a commitment to
                innovation and excellence, we exceed expectations and drive our
                clients' success.
              </div>
            </v-col>
          </v-row>
        </div>
        <div
          class="brand-list-wrapper my-16 d-flex justify-space-between align-center"
        >
          <img
            class="brand-logo"
            src="@/assets/project-page/logo-drfleurs.svg"
            alt=""
          />
          <img
            class="brand-logo"
            src="@/assets/project-page/logo-kazoku.svg"
            alt=""
          />
          <img
            class="brand-logo"
            src="@/assets/project-page/logo-og.svg"
            alt=""
          />
          <img
            class="brand-logo"
            src="@/assets/project-page/logo-proman.svg"
            alt=""
          />
          <img
            class="brand-logo"
            src="@/assets/project-page/logo-royalnatural.svg"
            alt=""
          />
          <img
            class="brand-logo"
            src="@/assets/project-page/logo-sumoji.svg"
            alt=""
          />
        </div>
        <ProjectList />
      </div>
    </section>
  </div>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from "vue";
// import LocomotiveScroll from "locomotive-scroll";

const scrollContainer = ref(null);
let locomotive = null;

// const scroll = new LocomotiveScroll();
// const target = document.querySelector("#home-page");

// scroll.scrollTo(target);

onMounted(() => {
  // locomotive = new LocomotiveScroll({
    // el: document.querySelector(".home-page"),
    // smooth: true,
  // });
});

onUnmounted(() => {
  if (locomotive) {
    locomotive.destroy();
  }
});
</script>

<style scoped lang="scss">
.home-page {
  transition: transform 0.6s ease;
  background: #0b0b0c;
  .banner-section {
    // height: 1000vh;
    .banner-content {
      position: relative;
      width: 100%;
      height: 100vh;
      .text {
        text-align: center;
        .heading {
          font-size: 70px;
          font-weight: 700;
          line-height: 70px;
          text-transform: uppercase;
          letter-spacing: -2px;
        }
        .subheading {
          font-size: 18px;
          font-weight: 400;
        }
      }
    }
    .field-section {
      position: relative;
      z-index: 100;
      border-radius: 80px;
      padding: 150px 250px;
      background: #fff;
      color: #121212;
      .description-wrapper {
        width: 100%;
        .description {
          font-size: 30px;
          font-weight: 400;
        }
      }
    }
    .title-section {
      position: relative;
      width: 100%;
      height: 50vh;

      .text {
        text-align: center;
        z-index: 100;
        .heading {
          font-size: 60px;
          font-weight: 400;
        }
      }
    }
    .approach-section {
      position: relative;
      width: 100%;
      height: 65vh;
      .approach-content {
        z-index: 100;
        padding: 0 200px;

        .heading {
          text-align: left;
          font-size: 60px;
          font-weight: 400;
        }
        .subheading {
          font-size: 18px;
          font-weight: 600;
        }
        .text {
          font-size: 16px;
          font-weight: 400;
          opacity: 60%;
        }
      }
    }

    .project-section {
      position: relative;
      z-index: 100;
      border-radius: 80px;
      padding: 150px 250px;
      background: #fff;
      color: #121212;
      .description-wrapper {
        width: 100%;
        .description {
          font-size: 30px;
          font-weight: 400;
        }
      }
      .brand-list-wrapper {
        width: 100%;
        overflow: hidden;
        .brand-logo {
          height: auto;
          width: auto;
        }
      }
    }
  }
}

/*! locomotive-scroll v4.1.3 | MIT License | https://github.com/locomotivemtl/locomotive-scroll */
// html.has-scroll-smooth {
//   overflow: hidden;
// }

// html.has-scroll-dragging {
//   -webkit-user-select: none;
//   -moz-user-select: none;
//   -ms-user-select: none;
//   user-select: none;
// }

// .has-scroll-smooth body {
//   overflow: hidden;
// }

// .has-scroll-smooth [data-scroll-container] {
//   min-height: 100vh;
// }

// [data-scroll-direction="horizontal"] [data-scroll-container] {
//   height: 100vh;
//   display: inline-block;
//   white-space: nowrap;
// }

// [data-scroll-direction="horizontal"] [data-scroll-section] {
//   display: inline-block;
//   vertical-align: top;
//   white-space: nowrap;
//   height: 100%;
// }

// .c-scrollbar {
//   position: absolute;
//   right: 0;
//   top: 0;
//   width: 11px;
//   height: 100%;
//   transform-origin: center right;
//   transition: transform 0.3s, opacity 0.3s;
//   opacity: 0;
// }
// .c-scrollbar:hover {
//   transform: scaleX(1.45);
// }
// .c-scrollbar:hover,
// .has-scroll-scrolling .c-scrollbar,
// .has-scroll-dragging .c-scrollbar {
//   opacity: 1;
// }
// [data-scroll-direction="horizontal"] .c-scrollbar {
//   width: 100%;
//   height: 10px;
//   top: auto;
//   bottom: 0;
//   transform: scaleY(1);
// }
// [data-scroll-direction="horizontal"] .c-scrollbar:hover {
//   transform: scaleY(1.3);
// }

// .c-scrollbar_thumb {
//   position: absolute;
//   top: 0;
//   right: 0;
//   background-color: black;
//   opacity: 0.5;
//   width: 7px;
//   border-radius: 10px;
//   margin: 2px;
//   cursor: -webkit-grab;
//   cursor: grab;
// }
// .has-scroll-dragging .c-scrollbar_thumb {
//   cursor: -webkit-grabbing;
//   cursor: grabbing;
// }
// [data-scroll-direction="horizontal"] .c-scrollbar_thumb {
//   right: auto;
//   bottom: 0;
// }
</style>
