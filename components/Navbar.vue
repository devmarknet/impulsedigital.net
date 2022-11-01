<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'NavbarComponent',
})
</script>

<template>
  <nav>
    <div class="container mx-auto px-6 pt-32 flex justify-center">
      <ul class="text-white/50 flex gap-14 text-sm uppercase">
        <li>
          <a href="#inicio">Início</a>
        </li>
        <li>
          <a href="#a-impulse">A Impulse</a>
        </li>
        <li>
          <a href="#servicos">Serviços</a>
        </li>
        <li>
          <a href="#nosso-trabalho">Nosso Trabalho</a>
        </li>
        <li>
          <a href="#beneficios">Benefícios</a>
        </li>
      </ul>
    </div>
  </nav>
</template>
