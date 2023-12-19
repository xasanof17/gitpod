<script setup>
import { workspaces } from "@/constants/workspaces"
</script>

<template>
  <section id="docs" class="container flex flex-col pb-[80px] md:pb-[120px] xl:pb-[160px]">
    <h2
      role="heading"
      class="mb-7 text-center text-xl font-bold text-primary md:text-3xl xl:mb-12 xl:text-5xl"
    >
      Get Started now
    </h2>
    <div class="mx-auto grid w-full max-w-lg grid-cols-1 gap-6 lg:max-w-full lg:grid-cols-2">
      <div
        class="flex flex-col items-center justify-center rounded-3xl bg-white px-2 pb-8 pt-12 text-center shadow-xl md:px-4 xl:px-14 xl:pb-20 xl:pt-14"
      >
        <h3 role="heading" class="mb-2 text-lg font-bold text-primary md:text-xl xl:text-2xl">
          Connect Git repository
        </h3>
        <p class="text-base font-normal text-primary/80 md:text-lg xl:text-xl">
          Select a Git provider to start with an existing project from any Git context.
        </p>
        <div class="my-10 flex flex-col space-y-4 xl:my-16">
          <a
            href="https://milleniumcompany.tech"
            target="_blank"
            class="flex items-center space-x-3 rounded-xl bg-[#FC6D26] px-7 py-2 text-base font-medium text-white shadow"
            ><svg
              xmlns="http://www.w3.org/2000/svg"
              width="28"
              height="28"
              viewBox="0 0 28 28"
              fill="none"
            >
              <g clip-path="url(#clip0_1_839)">
                <path d="M13.6108 27.2141L8.59601 10.9541H18.6181L13.6108 27.2141Z" fill="white" />
                <path
                  d="M25.6443 10.9541L27.1721 15.8941C27.3103 16.3431 27.1609 16.8381 26.796 17.1171L13.6117 27.2141L25.6443 10.9541Z"
                  fill="white"
                  fill-opacity="0.65"
                />
                <path
                  d="M25.6443 10.9541H18.6191L21.6431 1.16113C21.7971 0.661133 22.4719 0.661133 22.6324 1.16113L25.6443 10.9541Z"
                  fill="white"
                />
                <path
                  d="M1.57271 10.9541L0.0513757 15.8941C-0.0867577 16.3431 0.0625757 16.8381 0.427509 17.1171L13.6127 27.2141L1.57271 10.9541Z"
                  fill="white"
                  fill-opacity="0.65"
                />
                <path
                  d="M1.57266 10.9541H8.596L5.57946 1.16113C5.42453 0.661133 4.75066 0.661133 4.59013 1.16113L1.57266 10.9541Z"
                  fill="white"
                />
                <path
                  d="M13.6127 27.2141L8.59786 10.9541H1.57266L13.6127 27.2141Z"
                  fill="white"
                  fill-opacity="0.85"
                />
                <path
                  d="M13.6117 27.2141L25.6443 10.9541H18.6191L13.6117 27.2141Z"
                  fill="white"
                  fill-opacity="0.85"
                />
              </g>
              <defs>
                <clipPath id="clip0_1_839">
                  <rect width="28" height="28" fill="white" />
                </clipPath>
              </defs>
            </svg>
            <span>Continue with GitLab</span></a
          >
          <a
            href="https://milleniumcompany.tech"
            target="_blank"
            class="flex items-center space-x-3 rounded-xl bg-primary px-7 py-2 text-base font-medium text-white shadow"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="28"
              height="28"
              viewBox="0 0 28 28"
              fill="none"
            >
              <g clip-path="url(#clip0_1_855)">
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M14.0676 0.466797C10.7157 0.467811 7.47753 1.64141 4.95117 3.7708C2.39585 5.92585 0.707205 8.88193 0.18152 12.1204C-0.354352 15.3704 0.300638 18.6992 2.03338 21.5321C3.74434 24.3371 6.43685 26.4578 9.62428 27.5111C10.332 27.6389 10.5821 27.204 10.5821 26.8381V24.4787C6.65724 25.3215 5.82883 22.6129 5.82883 22.6129C5.57207 21.7781 5.01931 21.0574 4.26759 20.5773C2.9989 19.7252 4.3709 19.7252 4.3709 19.7252C4.81504 19.7877 5.23986 19.9492 5.61159 20.1965C5.98428 20.4439 6.29421 20.7724 6.51918 21.1569C6.70938 21.4985 6.96718 21.7991 7.27614 22.0427C7.73716 22.4095 8.30274 22.632 8.89772 22.6807C9.49271 22.7294 10.0889 22.6019 10.6072 22.3152C10.6622 21.6143 10.9683 20.9553 11.4703 20.4579C8.34787 20.1088 5.06897 18.916 5.06897 13.6445C5.04557 12.272 5.5606 10.9418 6.51049 9.92146C6.0892 8.72291 6.13834 7.41648 6.64855 6.25066C6.64855 6.25066 7.83035 5.87546 10.5126 7.67306C12.8146 7.04846 15.2501 7.04846 17.5521 7.67306C20.2353 5.87546 21.4084 6.25066 21.4084 6.25066C21.9259 7.40146 21.9877 8.70253 21.5812 9.89626C22.5306 10.9165 23.0452 12.2463 23.0218 13.6184C23.0218 18.9505 19.7352 20.1172 16.603 20.4317C16.939 20.7659 17.1988 21.1663 17.3639 21.6077C17.528 22.0483 17.5956 22.5187 17.5608 22.9881V26.7952C17.5608 27.2469 17.8119 27.596 18.5263 27.4597C21.6777 26.3791 24.33 24.2525 26.011 21.4584C27.7132 18.6369 28.3512 15.3324 27.8166 12.1073C27.292 8.89339 25.6219 5.95774 23.0952 3.80813C20.5973 1.68476 17.3937 0.499032 14.0676 0.466797Z"
                  fill="#F9F9F9"
                />
              </g>
              <defs>
                <clipPath id="clip0_1_855">
                  <rect width="28" height="28" fill="white" />
                </clipPath>
              </defs>
            </svg>
            <span>Continue with GitHub</span></a
          >
          <a
            href="https://milleniumcompany.tech"
            target="_blank"
            class="flex items-center space-x-3 rounded-xl bg-[#2684FF] px-7 py-2 text-base font-medium text-white shadow"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="28"
              height="28"
              viewBox="0 0 28 28"
              fill="none"
            >
              <g clip-path="url(#clip0_1_850)">
                <path
                  d="M0.8794 0.291504H0.869029C0.743437 0.292157 0.619453 0.323319 0.505554 0.382858C0.391656 0.442396 0.290531 0.528906 0.209097 0.636472C0.127662 0.744038 0.0678389 0.870122 0.0337182 1.0061C-0.00040251 1.14208 -0.00801556 1.28474 0.0113997 1.42434L3.69703 26.5998C3.7914 27.2333 4.28088 27.7023 4.85229 27.7082H22.5369C22.7448 27.7105 22.9465 27.6291 23.1057 27.4786C23.2649 27.3282 23.371 27.1187 23.4049 26.888L27.0905 1.429C27.1099 1.28951 27.1023 1.14694 27.0683 1.01105C27.0342 0.87515 26.9745 0.749125 26.8932 0.641579C26.8118 0.534033 26.7108 0.447499 26.5971 0.387888C26.4833 0.328276 26.3594 0.296991 26.2339 0.296171H26.2225L0.8794 0.291504ZM16.4018 18.4857H10.7572L9.22859 9.5035H17.7696L16.4007 18.4868L16.4018 18.4857Z"
                  fill="white"
                />
              </g>
              <defs>
                <clipPath id="clip0_1_850">
                  <rect width="28" height="28" fill="white" />
                </clipPath>
              </defs>
            </svg>
            <span>Continue with BitBucket</span></a
          >
        </div>
        <p class="text-base font-normal text-primary/80 md:text-lg xl:text-xl">
          Or prefix any GitLab, GitHub or Bitbucket URL with
        </p>
        <p
          class="mt-2 rounded-xl bg-[#FFE4BC] px-3 text-center text-lg font-normal text-primary/80"
        >
          gitpod.io/#
        </p>
      </div>
      <div
        class="flex flex-col rounded-3xl bg-white px-2 pb-8 pt-12 text-center shadow-xl md:px-4 xl:px-14 xl:pb-20 xl:pt-14"
      >
        <h3 role="heading" class="mb-2 text-lg font-bold text-primary md:text-xl xl:text-2xl">
          Launch an example workspace
        </h3>
        <p class="text-base font-normal text-primary/80 md:text-lg xl:text-xl">
          Dive into one of our example workspaces
        </p>
        <div class="mt-8 flex flex-col space-y-3">
          <div
            v-for="(workspace, index) in workspaces"
            :key="index"
            class="flex w-full items-center justify-between rounded-xl bg-[#F9F9F9] px-3 py-2 md:px-4"
          >
            <div class="flex items-center space-x-3 md:space-x-4">
              <!-- Use the workspace.img property for the image source -->
              <img
                :src="workspace.img"
                :alt="workspace.title"
                class="h-8 w-8 rounded-sm object-cover"
              />
              <!-- Use the workspace.title property for the workspace title -->
              <h4 class="text-base font-normal md:text-lg xl:text-xl">{{ workspace.title }}</h4>
            </div>
            <a
              href="https://milleniumcompany.tech"
              target="_blank"
              class="rounded-xl bg-primary px-5 py-1 text-base font-normal text-white"
              ><span class="block md:hidden">Launch</span>
              <span class="hidden md:block">Launch workspace</span></a
            >
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
