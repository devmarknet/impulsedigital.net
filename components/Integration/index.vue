<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'IntegrationComponent',
  mounted() {},
})
</script>

<template>
  <div class="container mx-auto p-6 text-center">
    <h2 class="title max-w-[502px] mx-auto">Integração entre os 03 pilares</h2>
    <ul class="flex px-24 my-12 relative">
      <li
        class="flex-1 z-50 flex flex-col gap-5 bg-transparent py-0.5 border-16 border-[#110C22] text-center ring-2 ring-offset-2 ring-offset-transparent ring-transparent rounded-lg"
        v-for="i in 3"
        :key="i"
      >
        <div
          class="flex-1 justify-center items-center z-50 flex flex-col gap-5 bg-[#110C22] m-0.5 py-12 px-6 text-center ring-2 ring-offset-2 ring-offset-transparent ring-transparent rounded-xl"
        >
          <svg
            class="mx-auto"
            width="60"
            height="60"
            viewBox="0 0 60 60"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <mask
              id="mask0_153_28"
              style="mask-type: alpha"
              maskUnits="userSpaceOnUse"
              x="0"
              y="0"
              width="60"
              height="60"
            >
              <rect width="60" height="60" fill="#D9D9D9" />
            </mask>
            <g mask="url(#mask0_153_28)">
              <path
                d="M52.499 40.875L51.4365 38.5625L49.124 37.5L51.4365 36.4375L52.499 34.125L53.5615 36.4375L55.874 37.5L53.5615 38.5625L52.499 40.875ZM39.999 37.625L37.624 32.375L32.374 30L37.624 27.625L39.999 22.375L42.374 27.625L47.624 30L42.374 32.375L39.999 37.625ZM52.499 25.875L51.4365 23.5625L49.124 22.5L51.4365 21.4375L52.499 19.125L53.5615 21.4375L55.874 22.5L53.5615 23.5625L52.499 25.875ZM19.499 54.25C18.4574 54.25 17.5724 53.885 16.844 53.155C16.114 52.4267 15.749 51.5417 15.749 50.5V9.5C15.749 8.45833 16.114 7.5725 16.844 6.8425C17.5724 6.11417 18.4574 5.75 19.499 5.75H40.499C41.5407 5.75 42.4257 6.11417 43.154 6.8425C43.884 7.5725 44.249 8.45833 44.249 9.5V17.25H42.499V13.375H17.499V46.625H42.499V42.75H44.249V50.5C44.249 51.5417 43.884 52.4267 43.154 53.155C42.4257 53.885 41.5407 54.25 40.499 54.25H19.499ZM17.499 48.375V50.5C17.499 51 17.7074 51.4583 18.124 51.875C18.5407 52.2917 18.999 52.5 19.499 52.5H40.499C40.999 52.5 41.4574 52.2917 41.874 51.875C42.2907 51.4583 42.499 51 42.499 50.5V48.375H17.499ZM17.499 11.625H42.499V9.5C42.499 9 42.2907 8.54167 41.874 8.125C41.4574 7.70833 40.999 7.5 40.499 7.5H19.499C18.999 7.5 18.5407 7.70833 18.124 8.125C17.7074 8.54167 17.499 9 17.499 9.5V11.625ZM17.499 48.375V52.5V50.5V48.375Z"
                fill="url(#paint0_linear_153_28)"
              />
            </g>
            <defs>
              <linearGradient
                id="paint0_linear_153_28"
                x1="15.749"
                y1="29.9957"
                x2="61.7629"
                y2="29.9957"
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

          <h3 class="font-title uppercase text-4xl text-white">Objetivos</h3>
        </div>
      </li>
      <div class="absolute w-1/2 h-full box-animated block rounded-lg"></div>
    </ul>
    <p
      class="text-[28px] leading-[38px] text-white mx-auto text-extralight max-w-[850px]"
    >
      A integração desses tres setores, aplicada de forma personalizada e
      estratégica de acordo com seu negócio, garante que os resultados sejam
      consistentes e duradouros, alavancando sua empresa de forma constante e
      sustentavel.
    </p>
  </div>
</template>

<style lang="postcss" scoped>
.box-animated {
  background: radial-gradient(
    50% 140.87% at 50% 49.99%,
    #ffffff 0%,
    rgba(255, 255, 255, 0) 100%
  );
  opacity: 1;
  left: 10%;
  right: auto;

  transition: ease-in-out 0.25s;
  animation: move infinite 3s;
}

@keyframes move {
  0 {
    left: 0%;
    opacity: 0;
  }
  50% {
    left: 40%;
    opacity: 1;
  }
  100% {
    left: 10%;
    opacity: 1;
  }
}
</style>
