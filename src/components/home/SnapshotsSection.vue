<template>
  <section class="px-4 lg:px-8 py-16 relative">
    <div class="flex gap-8 flex-col md:flex-row">
      <h1 class="uppercase text-5xl mb-4 font-semibold">My Life in Snapshots</h1>
    </div>
    <div class="grid-cols-2 md:grid-cols-5 grid mb-8 gap-4">
      <div class="grid grid-cols-1 md:hidden gap-4">
        <img
          v-for="(n, i) in [img1, img2, img3, img4, img5]"
          :key="i"
          :src="n"
          :alt="n + ''"
          class="rounded-xl"
        />
      </div>
      <div class="grid grid-cols-1 md:hidden gap-4">
        <img
          v-for="(n, i) in [img6, img7, img8, img9, img10]"
          :key="i"
          :src="n"
          :alt="n + ''"
          class="rounded-xl"
        />
      </div>

      <div
        v-for="(n, i) in [
          [img1, img2],
          [img3, img4],
          [img5, img6],
          [img7, img8],
          [img9, img10],
        ]"
        :key="i"
        class="hidden md:flex flex-col gap-4"
      >
        <img :src="n[0]" :alt="n[0] + ''" class="rounded-xl" />
        <img v-if="n[1]" :src="n[1]" :alt="n[1] + ''" class="rounded-xl" />
      </div>
    </div>
    <div class="bg-neutral-300 h-64 w-64 rounded-full absolute top-0 left-0 mt-16 -z-20"></div>
  </section>
</template>

<script lang="ts">
import img1 from '@/assets/gallery/img_01.jpg'
import img2 from '@/assets/gallery/img_02.jpg'
import img3 from '@/assets/gallery/img_03.jpg'
import img4 from '@/assets/gallery/img_04.jpg'
import img5 from '@/assets/gallery/img_05.jpg'
import img6 from '@/assets/gallery/img_06.jpg'
import img7 from '@/assets/gallery/img_07.jpg'
import img8 from '@/assets/gallery/img_08.jpg'
import img9 from '@/assets/gallery/img_09.jpg'
import img10 from '@/assets/gallery/img_10.jpg'
export default {
  data() {
    return {
      img1,
      img2,
      img3,
      img4,
      img5,
      img6,
      img7,
      img8,
      img9,
      img10,
    }
  },
  methods: {
    imgName(n: number) {
      return n < 10 ? '0' + n : n
    },
  },
}
</script>

<style></style>
