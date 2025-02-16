<template>
  <section class="h-screen px-12 lg:px-32 py-32 mb-8">
    <div class="w-full md:w-1/2 h-full flex flex-col md:justify-center">
      <h1 class="uppercase text-5xl xl:text-7xl mb-4 font-semibold">CAPTURING BEAUTY PHOTO</h1>
      <p class="capitalize xl:w-1/2 text-stone-500">
        a camera is an optical instrument that captures a visual image at their most basic, cameras
        are sealed
      </p>
      <div class="flex mt-3 gap-8">
        <a href="#">
          <i class="fa-brands fa-instagram socialIcon"></i>
        </a>
        <a href="#">
          <i class="fa-brands fa-linkedin socialIcon"></i>
        </a>
        <a href="#">
          <i class="fa-brands fa-facebook socialIcon"></i>
        </a>
        <a href="#">
          <i class="fa-brands fa-dribbble socialIcon"></i>
        </a>
        <a href="#">
          <i class="fa-brands fa-pinterest socialIcon"></i>
        </a>
      </div>
    </div>

    <div class="absolute bottom-0 right-0 overflow-hidden h-2/5 sm:h-1/2 md:h-3/5 lg:h-4/6 -z-50">
      <img src="@/assets/image.jpg" alt="img" class="h-full" />
    </div>
  </section>
</template>

<script lang="ts">
export default {}
</script>

<style></style>
