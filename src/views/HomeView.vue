<template>
  <div style="min-height: 100px">
    <navbar-element></navbar-element>
  </div>

  <!-- <main-section></main-section> -->

  <about-section id="about"></about-section>

  <aspirations-section id="aspirations"></aspirations-section>

  <snapshots-section id="snapshots"></snapshots-section>

  <contact-section id="contact"></contact-section>

  <footer-element></footer-element>
</template>

<script lang="ts">
import NavbarElement from '../components/NavbarElement.vue'
// import MainSection from '../components/home/MainSection.vue'
import AboutSection from '../components/home/AboutSection.vue'
import AspirationsSection from '../components/home/AspirationsSection.vue'
import SnapshotsSection from '../components/home/SnapshotsSection.vue'
import ContactSection from '../components/home/ContactSection.vue'
import FooterElement from '../components/NavbarElement.vue'

export default {
  components: {
    FooterElement,
    NavbarElement,
    // MainSection,
    AboutSection,
    AspirationsSection,
    SnapshotsSection,
    ContactSection,
  },
}
</script>

<style></style>
