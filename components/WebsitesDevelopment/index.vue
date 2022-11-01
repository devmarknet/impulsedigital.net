<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'WebsitesDevelopment',
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
        <li class="text-2xl">Sites responsivos</li>
        <li class="text-2xl">Layout Personalizado</li>
        <li class="text-2xl">Sites otimizados e gerenciáveis</li>
        <li class="text-2xl max-w-[446px]">
          Integração com Google Analytics e com ferramentas de email marketing
        </li>
      </ul>
    </div>
  </div>
</template>
