<template>
  <section class="px-4 lg:px-8 py-16 relative">
    <div class="flex gap-8 flex-col md:flex-row">
      <h1 class="uppercase text-5xl mb-4 font-semibold">My Life in Snapshots</h1>
    </div>
    <div class="grid-cols-2 md:grid-cols-5 grid mb-8 gap-4">
      <div class="grid grid-cols-1 md:hidden gap-4">
        <img
          v-for="(n, i) in [1, 2, 3, 4, 5]"
          :key="i"
          :src="'/src/assets/gallery/img_' + imgName(n) + '.jpg'"
          :alt="n + ''"
          class="rounded-xl"
        />
      </div>
      <div class="grid grid-cols-1 md:hidden gap-4">
        <img
          v-for="(n, i) in [6, 7, 8, 9, 10]"
          :key="i"
          :src="'/src/assets/gallery/img_' + imgName(n) + '.jpg'"
          :alt="n + ''"
          class="rounded-xl"
        />
      </div>

      <div
        v-for="(n, i) in [
          [1, 2],
          [3, 4],
          [5, 6],
          [7, 8],
          [9, 10],
        ]"
        :key="i"
        class="hidden md:flex flex-col gap-4"
      >
        <img
          :src="'/src/assets/gallery/img_' + imgName(n[0]) + '.jpg'"
          :alt="n[0] + ''"
          class="rounded-xl"
        />
        <img
          v-if="n[1]"
          :src="'/src/assets/gallery/img_' + imgName(n[1]) + '.jpg'"
          :alt="n[1] + ''"
          class="rounded-xl"
        />
      </div>
    </div>
    <div class="bg-neutral-300 h-64 w-64 rounded-full absolute top-0 left-0 mt-16 -z-20"></div>
  </section>
</template>

<script lang="ts">
export default {
  methods: {
    imgName(n: number) {
      return n < 10 ? '0' + n : n
    },
  },
}
</script>

<style></style>
