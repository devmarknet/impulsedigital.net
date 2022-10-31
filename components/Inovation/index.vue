<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'InovationComponent',
})
</script>

<template>
  <div>
    <div class="content p-6">
      <img
        :src="require('~/assets/svg/rocket-inovation.jpeg')"
        alt="Rocket Inovation Image"
      />
      <div class="text-white flex flex-col gap-5">
        <h2 class="font-title text-3xl uppercase">
          Inovação para atender a necessidade da sua empresa
        </h2>
        <p class="text-xl font-light">
          Conosco você terá soluções completas e inovadoras para a sua empresa
          subir de nível
        </p>
        <a
          class="bg-[#F2632D] text-white py-4 px-10 w-max rounded-full uppercase text-sm"
          href="#action"
          >Contate-nos</a
        >
      </div>
    </div>
  </div>
</template>
