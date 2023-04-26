<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'ServicesComponent',
  data() {
    return {
      items: [
        {
          symbol: 'objetivos.svg',
          title: 'Objetivos',
          text: 'Sabe aquele bate-papo para nos conhecer e trocar ideias? Pois bem, nosso primeiro passo é conhecer a realidade da sua empresa, seus objetivos, gargalos e necessidades.',
        },
        {
          symbol: 'produtos-e-servicos.svg',
          title: 'Produtos e Serviços',
          text: 'Para apontarmos soluções eficientes, precisamos conhecer seus produtos e serviços a fim de traçar estratégias de vendas.',
        },
        {
          symbol: 'vendas.svg',
          title: 'Vendas',
          text: 'Vamos analisar as suas vendas, seu faturamento, fluxo de caixa, frequência e também os perfis do seu público-alvo e das suas personas.',
        },
        {
          symbol: 'ferramentas.svg',
          title: 'Ferramentas',
          text: 'Identificarmos suas atuais ferramentas de comércio, contato e divulgação online, analisando sua eficácia e se estão de acordo com o que você realmente precisa.',
        },
        {
          symbol: 'posicionamento-digital.svg',
          title: 'Posicionamento Digital',
          text: 'Outro passo importante é verificar como está a sua presença digital nas mídias sociais. Analisaremos sua identidade visual aplicada ao marketing digital.',
        },
        {
          symbol: 'plano-de-acao.svg',
          title: 'Plano de Ação',
          text: 'Após o diagnóstico, elaboraremos um plano de ação personalizado, focado na sua realidade, objetivos e com o know-all de quem entende de presença digital e resultados.',
        },
      ],
    }
  },
})
</script>

<template>
  <div id="servicos" class="flex flex-col gap-8">
    <div class="container text-white p-6 text-center">
      <span class="uppercase opacity-50">Serviços</span>
      <h2 class="title my-5">Diagnóstico para o seu negócio</h2>
      <p class="text-cover">O passo a passo em busca de resultados</p>
    </div>
    <div class="container flex justify-center ">
      <ul class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 p-6 gap-20 ">
        <li
          class="flex flex-col gap-5 max-w-[426px]"
          v-for="i in items"
          :key="i"
        >
          <div class="flex items-center gap-4">
            <img
              class="w-8 h-8"
              :src="require(`~/assets/svg/${i.symbol}`)"
              alt="Ads Click Icon"
            />
            <h3 class="text-white font-title uppercase text-3xl">
              {{ items.indexOf(i) + 1 }}.{{ i.title }}
            </h3>
          </div>
          <p class="text-white/50 font-light">
            {{ i.text }}
          </p>
        </li>
      </ul>
    </div>
  </div>
</template>
