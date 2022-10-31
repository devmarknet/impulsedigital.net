<script lang="ts">
import Vue, { PropOptions } from 'vue'

interface AboutData {
  title: string
  body: string
  actionUrl: string
  actionTitle: string
  image: string
}

export default Vue.extend({
  name: 'AboutComponent',
  props: {
    data: {
      type: Object,
      // required: true,
    } as PropOptions<AboutData>,
  },
})
</script>

<template>
  <div>
    <div class="content">
      <div class="p-6 flex flex-col gap-6">
        <img
          class="w-20"
          width="auto"
          height="auto"
          :src="require('~/assets/images/brand-symbol.png')"
          alt="Brand Symbol"
        />
        <h2 class="text-white text-2xl font-title font-bold uppercase">
          Para quem é a impulse
        </h2>
        <p class="text-white font-light text-xl">
          As melhores soluções pensadas para o seu negócio
        </p>
      </div>
      <ul class="flex flex-col gap-6 text-white p-6">
        <li>
          <img src="" alt="" />
          <h3 class="font-title text-xl uppercase">
            Negócios locais e <span>MEI</span>
          </h3>
          <p class="font-light text-white/50 mt-6">
            Para você que precisa gerar mais tráfego para o seu negócio local,
            captar mais leads qualificados e fortalecer o posicionamento da sua
            marca, considerando os hábitos de consumo da audiência na sua
            cidade.
          </p>
        </li>
        <li>
          <img src="" alt="" />
          <h3 class="font-title text-xl uppercase">
            Negócios locais e <span>MEI</span>
          </h3>
          <p class="font-light text-white/50 mt-6">
            Para você que precisa gerar mais tráfego para o seu negócio local,
            captar mais leads qualificados e fortalecer o posicionamento da sua
            marca, considerando os hábitos de consumo da audiência na sua
            cidade.
          </p>
        </li>
        <li>
          <img src="" alt="" />
          <h3 class="font-title text-xl uppercase">
            Negócios locais e <span>MEI</span>
          </h3>
          <p class="font-light text-white/50 mt-6">
            Para você que precisa gerar mais tráfego para o seu negócio local,
            captar mais leads qualificados e fortalecer o posicionamento da sua
            marca, considerando os hábitos de consumo da audiência na sua
            cidade.
          </p>
        </li>
      </ul>
    </div>
  </div>
</template>
