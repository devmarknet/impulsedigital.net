<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'ServicesComponent',
})
</script>

<template>
  <div>
    <div class="content text-white p-6">
      <span class="uppercase text-xs">Serviços</span>
      <h2 class="text-3xl font-title uppercase mt-3 mb-6">
        Diagnóstico para o seu negócio
      </h2>
      <p class="text-xl font-light">O passo a passo em busca de resultados</p>
    </div>
    <ul class="grid grid-col-3 p-6 gap-8">
      <li class="flex flex-col gap-5" v-for="i in 6" :key="i">
        <div class="flex items-center gap-4">
          <img
            class="w-8 h-8"
            :src="require('~/assets/svg/ads_click.svg')"
            alt="Ads Click Icon"
          />
          <h3 class="text-white font-title uppercase text-xl">
            {{ i }}. Objetivos
          </h3>
        </div>
        <p class="text-white/50 font-light">
          Sabe aquele bate-papo para nos conhecer e trocar ideias? Pois bem,
          nosso primeiro passo é conhecer a realidade da sua empresa, seus
          objetivos, gargalos e necessidades.
        </p>
      </li>
    </ul>
  </div>
</template>
