<template>
  <section id="services-section" class="px-12 lg:px-32 py-16 relative overflow-hidden">
    <div class="flex gap-8 flex-col md:flex-row">
      <h1 class="uppercase text-5xl mb-4 font-semibold">Aspirations</h1>
      <p class="capitalize xl:w-1/2 text-stone-500 mb-8">
        My goal is to blend
        <span style="font-weight: bolder">psychology, journalism, and computer science</span> into a
        meaningful career. By understanding human behavior, crafting compelling stories, and
        mastering C programming, I aim to create technology and content that empower and connect
        people. I want to bridge the gap between humanity and innovation, using my skills to make a
        positive impact through empathy, creativity, and technical expertise.
      </p>
    </div>

    <div class="flex flex-col md:flex-row md:gap-8">
      <div
        class="flex flex-row md:flex-col justify-between md:justify-start items-center md:items-start my-8 md:w-1/3"
      >
        <img src="@/assets/services/wedding.png" alt="Wedding" class="-z-50 md:mb-4" />
        <div class="w-2/3 text-right md:text-left md:w-full">
          <h1 class="uppercase text-2xl font-semibold">Wedding</h1>
          <p class="capitalize text-stone-500">
            My 'wedding' is not to a person but to a higher calling—a commitment to God, community,
            and spiritual growth.
          </p>
        </div>
      </div>

      <div
        class="flex flex-row md:flex-col justify-between items-center md:items-start my-8 md:w-1/3"
      >
        <div class="w-2/3 text-left md:w-full md:order-2">
          <h1 class="uppercase text-2xl font-semibold">Lifestyle</h1>
          <p class="capitalize text-stone-500">
            My lifestyle is rooted in faith, service, and celibacy. Living simply, I focus on
            spiritual growth and serving others, finding purpose and fulfillment through prayer,
            guidance, and acts of compassion.
          </p>
        </div>
        <img
          src="@/assets/services/lifestyle.png"
          alt="Lifestyle"
          class="-z-50 md:mb-4 md:order-1"
        />
      </div>

      <div
        class="flex flex-row md:flex-col justify-between items-center md:items-start my-8 md:w-1/3"
      >
        <div class="w-1/3">
          <img src="@/assets/services/moments.png" alt="Moments" class="-z-50 md:mb-4" />
        </div>
        <div class="w-2/3 text-right md:text-left md:w-full">
          <h1 class="uppercase text-2xl font-semibold">Moments</h1>
          <p class="capitalize text-stone-500">
            Every movement of my life is guided by faith, service, and devotion. Whether through
            community support, or acts of compassion, I strive to live purposefully, embracing a
            life dedicated to uplifting others.
          </p>
        </div>
      </div>
    </div>

    <div class="bg-neutral-300 h-64 w-64 rounded-full absolute top-0 -right-20 mt-16 -z-20"></div>
  </section>
</template>

<script lang="ts">
export default {}
</script>

<style></style>
