<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'WebsitesDevelopment',
  data() {
    return {
      items: [
        {
          symbol: 'sites-responsivos.svg',
          title: 'Sites Responsivos',
        },
        {
          symbol: 'layout-personalizado.svg',
          title: 'Layout Personalizado',
        },
        {
          symbol: 'sites-otimizados.svg',
          title: 'Sites Otimizados e Gerenciáveis',
        },
        {
          symbol: 'analytics.svg',
          title:
            'Integração com Google Analytics e com ferramentas de email marketing',
        },
      ],
    }
  },
})
</script>

<template>
  <div
    class="pt-40"
    :style="`background: url(${require('~/assets/images/development-bg.png')})`"
  >
    <!-- <video :src="require('~/assets/movie/development.mov')"></video> -->
    <div
      class="container p-6 flex flex-col xl:flex-row xl:justify-between xl:items-center gap-12"
    >
      <div class="text-white">
        <h2 class="title max-w-[580px]">
          Desenvolvimento de Websites Personalizados
        </h2>
        <p
          class="text-[28px] leading-[38px] max-w-[720px] font-extralight mt-6"
        >
          Destaque-se entre os concorrentes com um site personalizado para o
          <b>seu negócio</b>. Utilizamos algumas das mais modernas tecnologias
          para criar sites interativos e performáticos
        </p>
      </div>
      <ul class="text-white font-light flex flex-col gap-6">
        <li
          v-for="i in items"
          :key="items.indexOf(i)"
          class="text-2xl flex items-center gap-6 max-w-[510px]"
        >
          <img :src="require(`~/assets/svg/${i.symbol}`)" :alt="i.title" />
          <p>{{ i.title }}</p>
        </li>
      </ul>
    </div>
  </div>
</template>
