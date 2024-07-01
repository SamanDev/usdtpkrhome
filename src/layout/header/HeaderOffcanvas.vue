<script setup>
import { inject } from "vue";

import logo_1 from "/assets/img/logo/logo.png";

const propValue = inject("offcanvasOpen");
const emit = defineEmits(["setOffcanvasOpen"]);

const handleClose = () => {
  emit("setOffcanvasOpen", false);
};
</script>

<template>
  <div :class="propValue ? 'offcanvas-menu-visible' : ''">
    <div class="extra-info" :class="propValue ? 'active' : ''">
      <div class="close-icon menu-close">
        <button @click="handleClose(false)">
          <i class="far fa-window-close"></i>
        </button>
      </div>
      <div class="logo-side mb-30">
        <router-link to="/"><img :src="logo_1" alt="Logo" /></router-link>
      </div>
      <div class="side-info mb-30">
        <div class="contact-list mb-30">
          <h4>Online Players</h4>
          <p>112 Players</p>
        </div>
        <div class="contact-list mb-30">
          <h4>Active Tables</h4>
          <p>45 Tables</p>
        </div>
        <div class="contact-list mb-30">
          <h4>Chips on Tables</h4>
          <p>$55,434</p>
        </div>
      </div>
      <div class="side-info mb-30">
        <div class="social-icon-right mt-30">
          <a href="#"><i class="fab fa-facebook-f"></i></a>
          <a href="#"><i class="fab fa-twitter"></i></a>
          <a href="#"><i class="fab fa-google-plus-g"></i></a>
          <a href="#"><i class="fab fa-instagram"></i></a>
        </div>
      </div>
    </div>
    <div
      @click="handleClose(false)"
      class="offcanvas-overly"
      :class="propValue ? 'active' : ''"
    ></div>
  </div>
</template>
