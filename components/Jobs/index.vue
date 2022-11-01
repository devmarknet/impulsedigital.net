<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'JobsComponents',
})
</script>

<template>
  <div class="container mx-auto p-6 flex justify-center items-center">
    <img :src="require('~/assets/images/jobs.png')" />
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
        <li v-for="i in 4" :key="i" class="flex flex-col gap-5">
          <div class="flex items-center gap-4">
            <h3 class="font-title uppercase text-3xl text-[#F2632D]">
              Objetivos
            </h3>
          </div>
          <p class="text-white/50 font-light max-w-[456px] leading-[26px]">
            Sabe aquele bate-papo para nos conhecer e trocar ideias? Pois bem,
            nosso primeiro passo é conhecer a realidade da sua empresa, seus
            objetivos, gargalos e necessidades.
          </p>
        </li>
      </ul>
    </div>
  </div>
</template>
