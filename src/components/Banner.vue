<script setup>
import IconGitlab from "./icons/IconGitlab.vue"
import IconGithub from "./icons/IconGithub.vue"
import IconBucket from "./icons/IconBucket.vue"
import HeroImage from "@assets/hero.png"
</script>

<template>
  <section
    id="hero"
    class="container my-10 flex flex-col items-center justify-between space-y-10 lg:flex-row lg:space-y-0 xl:my-14"
  >
    <div class="flex flex-col items-center justify-center lg:items-start">
      <h1 class="text-3xl font-bold text-primary md:text-5xl xl:text-7xl">
        Always <br class="hidden lg:block" />
        Ready to Code
      </h1>
      <p
        class="my-5 w-full max-w-md text-center text-lg font-normal text-primary md:text-xl lg:text-start xl:my-7"
      >
        Spin up fresh, automated dev environments for each task, in the cloud, in seconds.
      </p>
      <div class="item-center flex space-x-6">
        <a href="#" class="yellow-btn"> Try Now </a>
        <p class="text-sm font-medium text-primary md:text-base">
          Open a workspace. <br />
          Start from any Git context.
        </p>
      </div>
      <div class="mt-5 flex items-center space-x-6">
        <a href="#">
          <IconGitlab />
        </a>
        <a href="https://github.com/xasanof17" target="_blank">
          <IconGithub />
        </a>
        <a href="#">
          <IconBucket />
        </a>
      </div>
    </div>
    <img
      :src="HeroImage"
      alt="hero"
      class="h-full min-h-[300px] w-full max-w-lg object-cover md:min-h-[400px] lg:max-w-[500px] xl:min-h-[650px] xl:max-w-[630px]"
    />
  </section>
</template>
