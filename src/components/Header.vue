<script setup>
import { ref, computed } from "vue"
import { links } from "@/constants/links"
import Logo from "@assets/logo.svg"
import IconMenu from "./icons/IconMenu.vue"
import IconClose from "./icons/IconClose.vue"

const isMenuOpen = ref(false)

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value
}

const IconComponent = computed(() => (isMenuOpen.value ? IconClose : IconMenu))
</script>

<script>
export default {
  data() {
    return {
      links
    }
  }
}
</script>

<template>
  <header class="sticky left-0 top-0 z-50 bg-white py-3 shadow">
    <nav class="container flex items-center justify-between">
      <a href="https://milleniumcompany.tech" target="_blank">
        <img :src="Logo" alt="GitPod" class="object-cover" />
      </a>
      <ul class="hidden items-center space-x-7 lg:flex">
        <li v-for="({ href, title }, key) in links" :key="key">
          <a :href="href" class="text-base font-medium text-primary hover:text-black">
            {{ title }}
          </a>
        </li>
      </ul>
      <a href="https://milleniumcompany.tech" target="_blank" class="hidden rounded-2xl bg-primary px-4 py-2 text-base text-white lg:block"
        >Login</a
      >
      <button type="button" class="flex items-center justify-center lg:hidden" @click="toggleMenu">
        <component :is="IconComponent" />
      </button>

      <div
        v-show="isMenuOpen"
        class="absolute left-0 top-20 z-10 flex h-screen w-full flex-col bg-white pt-10 lg:hidden"
      >
        <ul class="flex flex-col items-center justify-center space-y-7 lg:hidden">
          <li v-for="({ href, title }, key) in links" :key="key">
            <a
              :href="href"
              class="text-lg font-medium text-primary transition-all duration-300 hover:text-black hover:underline"
            >
              {{ title }}
            </a>
          </li>
        </ul>
      </div>
    </nav>
  </header>
</template>
