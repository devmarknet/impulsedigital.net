<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'InovationComponent',
})
</script>

<template>
  <div class="container mx-auto flex items-center p-6 -mt-56 gap-12 flex-col xl:flex-row ">
    <img
      :src="require('~/assets/images/rocket-inovation.png')"
      alt="Rocket Inovation Image"
    />
    <div class="text-white flex flex-col gap-8">
      <h2 class="title max-w-[550px]">
        Inovação para atender a necessidade da sua empresa
      </h2>
      <p class="text-cover max-w-[588px]">
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
</template>
