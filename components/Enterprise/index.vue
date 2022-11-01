<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'EnterpriseComponent',
})
</script>

<template>
  <div class="container flex items-center justify-between mx-auto p-6">
    <div>
      <div class="content">
        <h2 class="title max-w-[600px]">
          Sua empresa no caminho do crescimento
        </h2>
        <p class="text-white text-3xl font-extralight mt-6 max-w-[520px]">
          Uma estratégia de marketing completa focada em branding e resultados
        </p>
      </div>
      <ul class="text-white mt-12 flex flex-wrap gap-10 max-w-[788px]">
        <li v-for="i in 6" :key="i" class="xl:w-[360px] max-w-[360px]">
          <h3 class="text-3xl font-title font-extralight flex gap-4 uppercase">
            <svg
              width="40"
              height="40"
              viewBox="0 0 40 40"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <mask
                id="mask0_153_502"
                style="mask-type: alpha"
                maskUnits="userSpaceOnUse"
                x="0"
                y="0"
                width="40"
                height="40"
              >
                <rect width="40" height="40" fill="#D9D9D9" />
              </mask>
              <g mask="url(#mask0_153_502)">
                <path
                  d="M18.208 33.167H9.08299C8.41633 33.167 7.84699 32.9307 7.37499 32.458C6.90299 31.986 6.66699 31.4027 6.66699 30.708V9.16699C6.66699 8.47233 6.88899 7.88899 7.33299 7.41699C7.77766 6.94433 8.29166 6.70799 8.87499 6.70799H17.042C17.1807 6.06933 17.493 5.52766 17.979 5.08299C18.465 4.63899 19.0693 4.41699 19.792 4.41699C20.4587 4.41699 21.042 4.63899 21.542 5.08299C22.042 5.52766 22.3613 6.06933 22.5 6.70799H30.667C31.361 6.70799 31.9443 6.94433 32.417 7.41699C32.889 7.88899 33.125 8.47233 33.125 9.16699V16.5H31.708V9.16699C31.708 8.88899 31.597 8.64599 31.375 8.43799C31.153 8.22933 30.917 8.12499 30.667 8.12499H26.375V11.958H13.417V8.12499H9.08299C8.83299 8.12499 8.60399 8.22933 8.39599 8.43799C8.18733 8.64599 8.08299 8.88899 8.08299 9.16699V30.708C8.08299 30.986 8.18733 31.2293 8.39599 31.438C8.60399 31.646 8.83299 31.75 9.08299 31.75H18.208V33.167ZM25.833 32.083L20.042 26.25L21.042 25.25L25.833 30.042L35.5 20.417L36.5 21.417L25.833 32.083ZM20 8.45799C20.3887 8.45799 20.708 8.33299 20.958 8.08299C21.208 7.83299 21.333 7.51366 21.333 7.12499C21.333 6.73633 21.208 6.40999 20.958 6.14599C20.708 5.88199 20.3887 5.74999 20 5.74999C19.6113 5.74999 19.292 5.88199 19.042 6.14599C18.792 6.40999 18.667 6.73633 18.667 7.12499C18.667 7.51366 18.792 7.83299 19.042 8.08299C19.292 8.33299 19.6113 8.45799 20 8.45799Z"
                  fill="url(#paint0_linear_153_502)"
                />
              </g>
              <defs>
                <linearGradient
                  id="paint0_linear_153_502"
                  x1="6.66699"
                  y1="18.7895"
                  x2="40.8784"
                  y2="18.7895"
                  gradientUnits="userSpaceOnUse"
                >
                  <stop offset="0.03" stop-color="#F2A01E" />
                  <stop offset="0.22" stop-color="#F29C20" />
                  <stop offset="0.41" stop-color="#F19126" />
                  <stop offset="0.58" stop-color="#F07E30" />
                  <stop offset="0.76" stop-color="#EF633E" />
                  <stop offset="0.92" stop-color="#ED4251" />
                  <stop offset="1" stop-color="#EC305A" />
                </linearGradient>
              </defs>
            </svg>

            Gestão estratégica
          </h3>
          <p
            class="text-white/50 mt-6 leading-[26px] font-extralight max-w-[302px] pl-14"
          >
            Sugestão de vendas online, análise de resultados e consultorias
          </p>
        </li>
      </ul>
    </div>
    <img :src="require('~/assets/svg/upscaling.svg')" alt="" />
  </div>
</template>
