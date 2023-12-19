<script setup>
import Ben from "@assets/ben.png"
</script>

<template>
  <section id="usedBy" class="container my-[20%] flex flex-col">
    <h2
      role="heading"
      class="mb-7 text-center text-xl font-bold text-primary md:text-3xl xl:mb-12 xl:text-5xl"
    >
      Used by 400,000+ developers.
    </h2>
    <div class="flex items-center justify-between space-x-6">
      <div class="w-full max-w-sm rounded-2xl bg-white p-6 shadow-xl">
        <p class="text-base font-normal text-primary md:text-lg">GitPod is incredibly cool.</p>
        <p class="my-3 text-base font-normal text-primary md:text-lg">
          In my opinion, this is a big step in open source software contribution. I'm excited to see
          where we go from here.
        </p>
        <div class="flex items-center justify-start space-x-3">
          <img :src="Ben" alt="ben" class="h-12 w-12 rounded-full object-cover" />
          <div class="flex flex-col">
            <h3 class="text-base font-bold text-primary md:text-lg">Ben Halpern</h3>
            <p class="text-base font-normal text-primary md:text-lg">
              Creator and Co-founder <strong>@forem</strong> and <strong>@ThePracticalDev</strong>
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
