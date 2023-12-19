<script setup>
import { footerLinks } from "@/constants/footerLinks"
</script>

<script>
const currentYear = new Date().getFullYear().toString()
</script>

<template>
  <footer class="bg-white pt-12">
    <div class="mx-auto flex w-full flex-col px-4 xl:max-w-[900px]">
      <div class="grid grid-cols-1 gap-5 md:grid-cols-4">
        <div v-for="({ title, lists }, key) in footerLinks" :key="key" class="flex flex-col">
          <h3 class="mb-3 text-lg font-bold text-primary">{{ title }}</h3>
          <ul class="flex flex-col space-y-2">
            <li v-for="({ title, href }, key) in lists" :key="key">
              <a :href="href" class="text-base font-normal text-primary/80 hover:text-black">
                {{ title }}
              </a>
            </li>
          </ul>
        </div>
      </div>
      <div class="mt-7 flex flex-col items-center justify-between border-t py-5 md:flex-row">
        <p class="flex items-center space-x-3">
          <img src="/favicon.ico" alt="gitpod logo" class="h-8 w-8 object-cover" />
          <span class="text-base font-medium text-primary"
            >Copyright &copy;
            {{ currentYear }}
            <a
              href="https://milleniumcompany.tech"
              target="_blank"
              class="font-bold text-indigo-600"
              >Millenium Company</a
            ></span
          >
        </p>
        <a class="flex items-center space-x-3">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
          >
            <g clip-path="url(#clip0_1_68)">
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M0 12C0 5.37258 5.37258 0 12 0C18.6274 0 24 5.37258 24 12C24 18.6274 18.6274 24 12 24C5.37258 24 0 18.6274 0 12ZM11.6406 9.75375L11.6658 10.169L11.2461 10.1181C9.71843 9.92323 8.38383 9.26226 7.25067 8.15216L6.69668 7.60135L6.55399 8.0081C6.25181 8.91482 6.44487 9.87239 7.0744 10.5164C7.41015 10.8723 7.33461 10.9232 6.75544 10.7113C6.55399 10.6435 6.37772 10.5927 6.36093 10.6181C6.30218 10.6774 6.50363 11.4486 6.66311 11.7536C6.88134 12.1773 7.32621 12.5925 7.81305 12.8383L8.22435 13.0332L7.73751 13.0417C7.26746 13.0417 7.25067 13.0501 7.30103 13.2281C7.46891 13.7789 8.13201 14.3636 8.87066 14.6178L9.39108 14.7958L8.93781 15.067C8.26631 15.4568 7.4773 15.6771 6.68829 15.694C6.31057 15.7025 6 15.7364 6 15.7618C6 15.8466 7.02404 16.3211 7.61999 16.5075C9.40786 17.0584 11.5315 16.8211 13.1263 15.8805C14.2595 15.211 15.3926 13.8806 15.9214 12.5925C16.2068 11.9062 16.4922 10.652 16.4922 10.0503C16.4922 9.66054 16.5174 9.60969 16.9874 9.14362C17.2644 8.87245 17.5246 8.57586 17.575 8.49112C17.6589 8.33011 17.6505 8.33011 17.2224 8.47417C16.509 8.72839 16.4083 8.6945 16.7608 8.31317C17.021 8.042 17.3316 7.5505 17.3316 7.40645C17.3316 7.38102 17.2057 7.42339 17.063 7.49966C16.9119 7.5844 16.5761 7.71151 16.3243 7.78778L15.8711 7.93184L15.4598 7.65219C15.2331 7.49966 14.9142 7.33018 14.7463 7.27934C14.3182 7.1607 13.6635 7.17765 13.2774 7.31323C12.2282 7.69456 11.5651 8.67755 11.6406 9.75375Z"
                fill="url(#paint0_linear_1_68)"
              />
            </g>
            <defs>
              <linearGradient
                id="paint0_linear_1_68"
                x1="3.45"
                y1="3.45"
                x2="21.107"
                y2="22.6608"
                gradientUnits="userSpaceOnUse"
              >
                <stop stop-color="#FFAD33" />
                <stop offset="1" stop-color="#FF8A00" />
              </linearGradient>
              <clipPath id="clip0_1_68">
                <rect width="24" height="24" fill="white" />
              </clipPath>
            </defs>
          </svg>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
          >
            <g clip-path="url(#clip0_1_60)">
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M12.0575 6.36076e-06C9.19512 -0.00296524 6.42524 1.03535 4.24425 2.92889C2.06326 4.82242 0.61373 7.4474 0.155424 10.3334C-0.302881 13.2194 0.259995 16.1778 1.74318 18.6784C3.22637 21.179 5.53292 23.0584 8.24948 23.9798C8.85581 24.0931 9.07024 23.7079 9.07024 23.3831C9.07024 23.0584 9.07024 22.3182 9.07024 21.291C5.70585 22.0387 4.996 19.637 4.996 19.637C4.77281 18.8926 4.29863 18.2531 3.65764 17.8319C2.57068 17.0766 3.74637 17.0766 3.74637 17.0766C4.1274 17.1316 4.49118 17.2744 4.81017 17.4942C5.12916 17.7141 5.395 18.0052 5.58754 18.3455C5.75115 18.6485 5.97172 18.9155 6.23661 19.1312C6.5015 19.347 6.80549 19.5071 7.13113 19.6026C7.45677 19.698 7.79765 19.7268 8.13422 19.6874C8.47079 19.6479 8.79642 19.541 9.09242 19.3726C9.13883 18.7513 9.40107 18.1674 9.83185 17.7262C7.15513 17.4165 4.34531 16.3591 4.34531 11.684C4.32693 10.4627 4.76906 9.28099 5.58015 8.38349C5.21891 7.3216 5.26113 6.15988 5.69846 5.12828C5.69846 5.12828 6.71147 4.79596 9.01109 6.38958C10.9858 5.83579 13.0701 5.83579 15.0448 6.38958C17.3444 4.79596 18.35 5.12828 18.35 5.12828C18.7935 6.14897 18.8462 7.30235 18.4979 8.36083C19.309 9.25834 19.7511 10.4401 19.7328 11.6614C19.7328 16.3893 16.9156 17.4241 14.2314 17.7035C14.5192 17.999 14.7415 18.3543 14.8831 18.7452C15.0247 19.1361 15.0824 19.5536 15.0522 19.9693C15.0522 21.6158 15.0522 22.9451 15.0522 23.3454C15.0522 23.7456 15.2666 24.0553 15.8804 23.9345C18.566 22.9888 20.838 21.1041 22.295 18.6132C23.752 16.1223 24.3002 13.1856 23.8428 10.3219C23.3854 7.45814 21.9518 4.85167 19.7953 2.96295C17.6388 1.07422 14.8982 0.024771 12.0575 6.36076e-06Z"
                fill="url(#paint0_linear_1_60)"
              />
            </g>
            <defs>
              <linearGradient
                id="paint0_linear_1_60"
                x1="3.45"
                y1="3.45"
                x2="21.107"
                y2="22.6608"
                gradientUnits="userSpaceOnUse"
              >
                <stop stop-color="#FFAD33" />
                <stop offset="1" stop-color="#FF8A00" />
              </linearGradient>
              <clipPath id="clip0_1_60">
                <rect width="24" height="24" fill="white" />
              </clipPath>
            </defs>
          </svg>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
          >
            <g clip-path="url(#clip0_1_64)">
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M0 11.7908C0 5.2781 5.48155 0 11.9919 0C18.4953 0 23.7804 5.48618 23.7804 11.9965C23.7804 18.5069 18.5 23.9884 11.9896 23.9884L0 24V11.7908ZM5.8306 8.13398C7.14804 5.9215 9.53234 4.56533 12.1074 4.56381H12.1143C15.0968 4.56526 17.7792 6.37901 18.8915 9.14636C20.0038 11.9137 19.3228 15.0793 17.1709 17.1445C15.019 19.2096 11.8281 19.7599 9.1088 18.5347L4.36012 19.6074L5.68254 15.3535C4.45692 13.0889 4.51317 10.3465 5.8306 8.13398Z"
                fill="url(#paint0_linear_1_64)"
              />
            </g>
            <defs>
              <linearGradient
                id="paint0_linear_1_64"
                x1="3.41843"
                y1="3.45"
                x2="21.0884"
                y2="22.499"
                gradientUnits="userSpaceOnUse"
              >
                <stop stop-color="#FFAD33" />
                <stop offset="1" stop-color="#FF8A00" />
              </linearGradient>
              <clipPath id="clip0_1_64">
                <rect width="24" height="24" fill="white" />
              </clipPath>
            </defs>
          </svg>
        </a>
      </div>
    </div>
  </footer>
</template>
