<template>
  <!-- Navbar start -->
  <nav class="w-screen fixed bg-opacity-90 bg-white p-4 lg:px-20 flex justify-between z-50">
    <!-- Logo start -->
    <div class="h-full flex flex-col justify-center">
      <p class="tracking-widest font-semibold">I'm</p>
      <p class="tracking-widest font-light">CHANDAN</p>
    </div>
    <!-- Logo end -->

    <!-- Toggler start -->
    <button role="menubar" class="md:hidden" @click="navToggle()">
      <i class="fa-solid fa-bars text-2xl"></i>
    </button>
    <!-- Toggler end -->

    <!-- Menu content start -->
    <div
      class="absolute left-0 right-0 translate-y-16 bg-opacity-90 bg-white md:bg-none md:bg-opacity-0 shadow hidden md:flex flex-col gap-4 items-center p-4 md:flex-row md:static md:shadow-none md:translate-y-0"
      role="menu"
      aria-expanded="false"
    >
      <a href="#" role="menuitem">
        <p class="mx-4">Home</p>
      </a>

      <a href="#about" role="menuitem">
        <p class="mx-4">About</p>
      </a>

      <a href="#snapshots" role="menuitem">
        <p class="mx-4">Snapshots</p>
      </a>
      <a href="#contact" role="menuitem">
        <p class="mx-4">Contact</p>
      </a>
    </div>
  </nav>
</template>

<script lang="ts">
export default {
  methods: {
    navToggle() {
      const menu = document.querySelector("[role='menu']")
      const isExpanded = menu?.getAttribute('aria-expanded')
      menu?.setAttribute('aria-expanded', `${!isExpanded}`)
      menu?.classList.toggle('hidden')
      menu?.classList.toggle('flex')
    },
  },
}
</script>

<style></style>
