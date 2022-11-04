<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'EnterpriseComponent',
  data() {
    return {
      items: [
        {
          symbol: 'planejamento.svg',
          title: 'Planejamento',
          text: 'Plano de marketing organizando ideia, objetivos e ações',
        },
        {
          symbol: 'gerenciamento-de-midias.svg',
          title: 'Gerenciamento De Mídias',
          text: 'Criação de conteúdo para Facebook e Instagram, programação de conteúdo monitoramento e análise e métricas.',
        },
        {
          symbol: 'gestao-estrategica.svg',
          title: 'Gestão Estratégica',
          text: 'Plano de marketing organizando ideia, objetivos e ações',
        },
        {
          symbol: 'digital-branding.svg',
          title: 'Digital Branding',
          text: 'Diagnósitco de posicionamento, branding book da marca, design da marca para mídias sociais',
        },
        {
          symbol: 'design-prototipacao.svg',
          title: 'Design e Protipação',
          text: 'UI Design, Criação e Redesign de logo, landing page',
        },
        {
          symbol: 'gestao-de-trafego.svg',
          title: 'Gestão de tráfego',
          text: 'Facebook ads, Google ads, Google Analytics',
        },
      ],
    }
  },
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
        <li v-for="i in items" :key="i" class="xl:w-[360px] max-w-[360px]">
          <h3 class="text-3xl font-title font-extralight flex gap-4 uppercase">
            <img :src="require(`~/assets/svg/${i.symbol}`)" :alt="i.title" />

            {{ i.title }}
          </h3>
          <p
            class="text-white/50 mt-6 leading-[26px] font-extralight max-w-[302px] pl-14"
          >
            {{ i.text }}
          </p>
        </li>
      </ul>
    </div>
    <img :src="require('~/assets/svg/upscaling.svg')" alt="" />
  </div>
</template>
