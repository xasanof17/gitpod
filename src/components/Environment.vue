<script setup>
import DevEnvImage from "@assets/dev-environment.png"
</script>

<template>
  <section id="environment" class="container mb-10 grid grid-cols-1 gap-x-16 lg:grid-cols-2">
    <div class="flex flex-col">
      <h2 class="mb-2 text-xl font-bold text-primary md:text-2xl xl:text-4xl">
        Think CI/CD for dev environments
      </h2>
      <p class="text-base font-normal text-primary/80 md:text-lg xl:text-xl">
        We invented prebuilds so application code, configuration and infrastructure can all be
        stored as machine-executable code in your git repositories and applied to dev environments
        automatically and continuously.
      </p>
      <div class="my-10 flex items-center space-x-3 lg:mb-20 lg:mt-auto">
        <p class="yellow-btn px-5 py-1 text-sm">More on prebuilds</p>
        <p class="pink-btn px-5 py-1 text-sm">Documentation</p>
      </div>
    </div>
    <img
      :src="DevEnvImage"
      alt="Dev Environment Image"
      class="mx-auto h-full w-full max-w-lg lg:max-w-full"
    />
  </section>
</template>
