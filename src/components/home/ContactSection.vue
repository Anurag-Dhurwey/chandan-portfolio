<template>
  <section class="px-12 lg:px-32 py-16 relative">
    <h1 class="uppercase text-5xl mb-4 font-semibold">Contact us</h1>

    <div class="grid grid-cols-1 md:grid-cols-2 w-full">
      <div class="hidden md:flex justify-center items-center">
        <img src="/src/assets/camera.png" alt="" />
      </div>
      <div class="flex flex-col w-full items-center">
        <label for="user_email" class="text-stone-500 text-left">E-mail address</label>
        <input
          type="email"
          name="user_email"
          id="user_email"
          class="bg-stone-200 py-2 px-4 w-full mb-6 xl:w-1/2"
        />

        <label for="user_message" class="text-stone-500 text-left">Message</label>
        <textarea
          name="user_message"
          id="user_message"
          cols="30"
          rows="10"
          class="bg-stone-200 py-2 px-4 w-full mb-6 xl:w-1/2"
        ></textarea>

        <input
          value="Send"
          type="button"
          class="bg-stone-200 py-2 px-4 w-full mb-6 xl:w-1/2 cursor-pointer"
        />
      </div>
    </div>
    <div
      class="bg-neutral-200 h-44 w-44 md:h-52 md:w-52 rounded-full absolute -top-20 left-0 mt-16 -z-20"
    ></div>
  </section>
</template>

<script lang="ts">
export default {}
</script>

<style></style>
