<template>
  <div class="footer-section">
    <div class="footer-content d-flex flex-column justify-center align-center">
      <div class="heading mb-6">
        Ready to embark on your <br />
        digital journey?
      </div>
      <TrimindButton :text="'Start a project'" />
    </div>
    <hr class="mt-16 mb-5" />
    <div class="social-wrapper">
      <v-row>
        <v-col cols="12" class="d-flex justify-space-between">
          <img src="@/assets/logo.svg" alt="" width="130px" />
          <div class="button-wrapper">
            <v-btn class="ml-3" height="40" variant="text" width="40px">
              <img src="@/assets/footer/instagram.webp" alt="" width="100%" />
            </v-btn>

            <v-btn class="ml-3" height="40" variant="text" width="40px">
              <img src="@/assets/footer/email.webp" alt="" width="100%" />
            </v-btn>
            <v-btn class="ml-3" height="40" variant="text" width="40px">
              <img src="@/assets/footer/whatsapp.webp" alt="" width="100%" />
            </v-btn>
          </div>
        </v-col>
      </v-row>
      <hr class="mt-5 mb-16" />
      <v-row>
        <v-col cols="12 mb-0 pb-0">
          <div class="text text-center">
            © Copyright 2024 TriMind Studio. All Rights Reserved.
          </div>
        </v-col>
      </v-row>
    </div>
  </div>
</template>
<script setup></script>
<style lang="scss">
.footer-section {
  background: #0b0b0c;
  padding: 150px 250px 30px;
  hr {
    opacity: 15%;
  }
  .heading {
    font-size: 60px;
    line-height: 70px;
    font-weight: 400;
    color: #fff;
    text-align: center;
  }
  .social-wrapper {
    .text {
      font-size: 16px;
      color: #fff;
      opacity: 60%;
      text-align: right;
    }

    .v-btn {
      border-radius: 50%;
      border-color: #ffffffc0;
      min-width: unset !important;
      padding: 0 8px !important;
      .v-btn--size-default {
        min-width: unset !important;
        padding: 0 8px !important;
      }
    }
  }
}
</style>
