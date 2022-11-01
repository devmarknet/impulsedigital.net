<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'ServicesComponent',
})
</script>

<template>
  <div class="flex flex-col gap-8">
    <div class="container text-white p-6 text-center">
      <span class="uppercase opacity-50">Serviços</span>
      <h2 class="title my-5">Diagnóstico para o seu negócio</h2>
      <p class="text-cover">O passo a passo em busca de resultados</p>
    </div>
    <div class="container flex justify-center">
      <ul class="grid grid-cols-3 p-6 gap-20">
        <li class="flex flex-col gap-5 max-w-[426px]" v-for="i in 6" :key="i">
          <div class="flex items-center gap-4">
            <img
              class="w-8 h-8"
              :src="require('~/assets/svg/ads_click.svg')"
              alt="Ads Click Icon"
            />
            <h3 class="text-white font-title uppercase text-3xl">
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
  </div>
</template>
