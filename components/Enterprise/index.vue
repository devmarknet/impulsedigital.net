<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'EnterpriseComponent',
})
</script>

<template>
  <div>
    <div class="content p-6">
      <h2 class="text-white font-title uppercase text-3xl">
        Sua empresa no caminho do crescimento
      </h2>
      <p class="text-white text-xl mt-6">
        Uma estratégia de marketing completa focada em branding e resultados
      </p>
    </div>
    <ul class="text-white p-6 grid grid-cols-2 gap-4">
      <li v-for="i in 6" :key="i">
        <h3 class="font-title uppercase">Gerenciamento de mídias</h3>
        <p class="text-white/50 mt-4 font-light">
          Criação de conteúdo para Facebook e Instagram, programação de conteúdo
          monitoramento e análise e métricas.
        </p>
      </li>
    </ul>
  </div>
</template>
