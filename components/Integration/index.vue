<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'IntegrationComponent',
  data() {
    return {
      items: [
        {
          symbol: 'digital.svg',
          title: 'Digital',
        },
        {
          symbol: 'comercial.svg',
          title: 'Comercial',
        },
        {
          symbol: 'offline.svg',
          title: 'Offline',
        },
      ],
    }
  },
})
</script>

<template>
  <div class="container mx-auto p-6 text-center">
    <h2 class="title max-w-[502px] mx-auto">Integração entre os 03 pilares</h2>
    <ul class="flex flex-col sm:flex-row px-9 lg:px-24 my-12 relative">
      <li
        v-for="i in items"
        :key="i"
        class="flex-1 z-50 flex flex-col gap-5 bg-transparent py-0.5 border-16 border-[#110C22] text-center ring-2 ring-offset-2 ring-offset-transparent ring-transparent rounded-lg"
      >
        <div
          class="flex-1 justify-center items-center z-50 flex flex-col gap-5 bg-[#110C22] m-0.5 py-12 px-6 text-center ring-2 ring-offset-2 ring-offset-transparent ring-transparent rounded-xl"
        >
          <img :src="require(`~/assets/svg/${i.symbol}`)" :alt="i.title" />

          <h3 class="font-title uppercase text-4xl text-white">
            {{ i.title }}
          </h3>
        </div>
      </li>
      <div class="absolute w-1/2 h-full box-animated hidden sm:block rounded-lg "></div>
    </ul>
    <p
      class="text-[28px] leading-[38px] text-white mx-auto text-extralight lg:max-w-[850px]"
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
