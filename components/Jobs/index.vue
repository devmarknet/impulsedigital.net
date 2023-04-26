<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'JobsComponents',
  data() {
    return {
      jobs: [
        {
          title: 'Atração',
          text: 'Atrair as pessoas certas com o conteúdo e as conversas corretas direcionadas a elas, tornando você um consultor de confiança com quem elas desejam se engajar.',
        },
        {
          title: 'Conversão',
          text: 'Uma vez que você conseguiu atrair seu público, pode então, começar a pensar sobre a etapa de conversão, onde, em troca de conteúdo valioso e relevante, os visitantes te entregam informações e se tornam leads.',
        },
        {
          title: 'Venda',
          text: 'Depois de ter atraído e conduzido seus leads por todo o ciclo de compra, até chegar ao estágio de venda, o objetivo principal, deve ser transformá-lo em seu cliente.',
        },
        {
          title: 'Fidelização',
          text: 'Através da parceria entre o Inboud Marketing e o Marketing de Conteúdo traçamos estratégias para fidelizar seu cliente.',
        },
      ],
    }
  },
})
</script>

<template>
  <div id="nosso-trabalho" class="container mx-auto p-6 flex justify-center items-center flex-col lg:flex-row">
    <img class="hidden lg:block" :src="require('~/assets/images/jobs.png')" />
    <div class="xl:pt-32">
      <div class="content p-6 pt-12">
        <h2 class="title">Nosso Trabalho</h2>
        <p
          class="text-[28px] leading-[38px] mt-5 text-white max-w-[358px] text-extralight"
        >
          Conheça nosso método de Inbound Marketing
        </p>
      </div>
      <ul class="grid grid-col-3 p-6 gap-8">
        <li
          v-for="i in jobs"
          :key="jobs.indexOf(i)"
          class="flex flex-col gap-5"
        >
          <div class="flex items-center gap-4">
            <h3 class="font-title uppercase text-3xl text-[#F2632D]">
              {{ i.title }}
            </h3>
          </div>
          <p class="text-white/50 font-light max-w-[456px] leading-[26px]">
            {{ i.text }}
          </p>
        </li>
      </ul>
    </div>
  </div>
</template>
