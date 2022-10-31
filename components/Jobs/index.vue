<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'JobsComponents',
})
</script>

<template>
  <div>
    <div class="content p-6 pt-12">
      <h2 class="font-title text-3xl text-white uppercase">Nosso Trabalho</h2>
      <p class="text-white text-xl font-light mt-6">
        Conheça nosso método de Inbound Marketing
      </p>
    </div>
    <ul class="grid grid-col-3 p-6 gap-8">
      <li class="flex flex-col gap-5" v-for="i in 4" :key="i">
        <div class="flex items-center gap-4">
          <h3 class="font-title uppercase text-xl text-[#F2632D]">Objetivos</h3>
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
