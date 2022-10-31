<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'IntegrationComponent',
})
</script>

<template>
  <div>
    <div class="content p-6 pt-12">
      <h2 class="font-title text-3xl text-white uppercase text-center">
        Integração entre os 3 pilares
      </h2>
    </div>
    <ul class="grid grid-col-3 p-6 gap-8">
      <li
        class="flex flex-col gap-5 bg-[#110C22] py-10 px-6 text-center"
        v-for="i in 3"
        :key="i"
      >
        <h3 class="font-title uppercase text-xl text-[#F2632D]">Objetivos</h3>
      </li>
    </ul>
    <p class="text-white text-xl font-light text-center p-6">
      A integração desses tres setores, aplicada de forma personalizada e
      estratégica de acordo com seu negócio, garante que os resultados sejam
      consistentes e duradouros, alavancando sua empresa de forma constante e
      sustentavel.
    </p>
  </div>
</template>
