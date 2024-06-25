<template>
  <div class="project-list-wrapper d-flex flex-wrap ga-10">
    <v-row>
      <v-col
        v-for="(item, index) in projectList"
        :key="index"
        cols="6"
        md="6"
        lg="6"
        class="mb-5"
      >
        <div class="project-card">
          <v-card
            aspect-ratio="1"
            class="card-image d-flex align-center justify-center rounded-xl"
            :image="item.background"
          >
            <img :src="item.logo" alt="" width="200px" />
          </v-card>
        </div>

        <div class="project-info-wrapper mt-5">
          <div class="first-line d-flex justify-space-between">
            <div class="project-name text-mono">{{ item.name }}</div>
            <div class="project-year text-mono">{{ item.year }}</div>
          </div>

          <div class="second-line d-flex justify-space-between">
            <div class="project-location text-mono">{{ item.location }}</div>
            <div class="project-description">{{ item.description }}</div>
          </div>
        </div>
      </v-col>
    </v-row>
  </div>
</template>
<script setup>
import backgroundSumoji from "@/assets/project-page/list/background_sumoji.webp";
import logoSumoji from "@/assets/project-page/list/logo_sumoji.webp";

import backgroundDrfleurs from "@/assets/project-page/list/background_drfleurs.webp";
import logoDrfleurs from "@/assets/project-page/list/logo_drfleurs.webp";

import backgroundProman from "@/assets/project-page/list/background_proman.webp";
import logoProman from "@/assets/project-page/list/logo_proman.webp";

import backgroundKazoku from "@/assets/project-page/list/background_kazoku.webp";
import logoKazoku from "@/assets/project-page/list/logo_kazoku.webp";

import backgroundOrange from "@/assets/project-page/list/background_orangegrocer.webp";
import logoOrange from "@/assets/project-page/list/logo_orangegrocer.webp";

import backgroundRoyal from "@/assets/project-page/list/background_royalnatural.webp";
import logoRoyal from "@/assets/project-page/list/logo_royalnatural.webp";

const projectList = [
  {
    name: "SUMŌ-JI",
    location: "Jakarta, Indonesia",
    year: "2021",
    description: "Modern izakaya and sake lounge",
    background: backgroundSumoji,
    logo: logoSumoji,
  },
  {
    name: "dr. Fleurs",
    location: "Jakarta, Indonesia",
    year: "2019",
    description: "Florist and bouquet expertise",
    background: backgroundDrfleurs,
    logo: logoDrfleurs,
  },
  {
    name: "PROMAN",
    location: "Jakarta, Indonesia",
    year: "2023",
    description: "Property management app",
    background: backgroundProman,
    logo: logoProman,
  },
  {
    name: "Kazoku Hibachi Express",
    location: "Arkansas, USA",
    year: "2023",
    description: "Japanese hibachi restaurant",
    background: backgroundKazoku,
    logo: logoKazoku,
  },
  {
    name: "Orange Grocer",
    location: "CALIFORNIA, USA",
    year: "2023",
    description: "Online asian grocery market",
    background: backgroundOrange,
    logo: logoOrange,
  },
  {
    name: "Royal Natural",
    location: "Jakarta, Indonesia",
    year: "2020",
    description: "Health ingredient shop",
    background: backgroundRoyal,
    logo: logoRoyal,
  },
];
</script>
<style lang="scss">
.project-list-wrapper {
  .project-card {
    height: 400px;
    width: 100%;
    .card-image {
      height: 400px;
      width: 100%;
      .v-img__img--cover {
        object-fit: cover;
      }
    }
  }

  .first-line {
    font-weight: 600;
  }
  .second-line {
    opacity: 50%;
    .project-location {
      font-weight: 600;
    }
  }
}
</style>
