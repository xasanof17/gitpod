<script setup>
import CodeImage from "@assets/code.png"
import IconChromium from "./icons/IconChromium.vue"
import IconFirefox from "./icons/IconFirefox.vue"
</script>

<template>
  <section id="remote" class="container mb-[10%] mt-[40%] flex flex-col lg:mt-[20%]">
    <h2
      role="heading"
      class="mb-7 text-center text-xl font-bold text-primary md:text-3xl xl:mb-12 xl:text-5xl"
    >
      Remote first. Secure by design.
    </h2>
    <img
      :src="CodeImage"
      alt="code editor image"
      class="h-[250px] w-full md:h-[400px] lg:h-[600px] xl:h-[800px]"
    />
    <div class="mx-auto mt-6 flex w-full max-w-4xl flex-col items-center justify-center lg:mt-14">
      <p
        class="mx-auto mb-10 text-center text-base font-medium text-primary/80 md:text-lg xl:text-xl"
      >
        You no longer need an over-powered laptop to code, Gitpod works just as smoothly on a
        Chromebook or iPad. All you need is a browser. Gitpod centralizes all source code and never
        stores it on insecure machines and networks.
      </p>
      <div
        class="inline-flex flex-col items-center space-y-3 md:flex-row md:space-x-4 md:space-y-0"
      >
        <a href="#" class="flex items-center space-x-3 rounded-xl bg-white px-4 py-2 shadow-lg">
          <IconChromium />
          <span class="text-base font-bold text-primary">Chrome Extension</span>
        </a>
        <a href="#" class="flex items-center space-x-3 rounded-xl bg-white px-4 py-2 shadow-lg">
          <IconFirefox />
          <span class="text-base font-bold text-primary">Firefox Extension</span>
        </a>
      </div>
    </div>
  </section>
</template>
