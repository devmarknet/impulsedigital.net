<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'FormComponent',
})
</script>

<template>
  <div
    class="pb-32 pt-16"
    :style="`background: url(${require('~/assets/images/form-bg.png')})`"
  >
    <div class="container mx-auto p-6 flex items-center justify-between">
      <div>
        <h2 class="title">Contate-nos</h2>
        <p
          class="gradient-text font-title uppercase max-w-[510px] text-[40px] leading-[52px] py-6"
        >
          Inicie a jornada de sucesso de sua empresa entrando em contato conosco
        </p>
        <p class="text-3xl text-white max-w-[510px] font-thin">
          Somos especialistas em inovação para vendas que você está procurando
        </p>
        <ul class="text-white/50 flex flex-col gap-5 mt-16 max-w-[424px]">
          <li>Consolide sua presença digital</li>
          <li>
            Ferramentas que permitem ter previsibilidade e acompanhar o
            crescimento do seu negócio.
          </li>
          <li>Acompanhamento e relatórios mensais de vendas e marketing</li>
          <li>Equipe qualificada a serviço do seu negócio</li>
        </ul>
      </div>
      <div>
        <form class="flex flex-col gap-5">
          <label class="relative" for="">
            <span class="absolute py-2 px-4 text-xs text-gray-400 font-medium"
              >Email</span
            >
            <input
              type="text"
              class="pt-6 pb-3 px-4 w-[570px] rounded-md"
              placeholder="Seu melhor email"
            />
          </label>
          <label class="relative" for="">
            <span class="absolute py-2 px-4 text-xs text-gray-400 font-medium"
              >Seu nome</span
            >
            <input
              type="text"
              class="pt-6 pb-3 px-4 w-[570px] rounded-md"
              placeholder="Seu nome completo"
            />
          </label>
          <label class="relative" for="">
            <span class="absolute py-2 px-4 text-xs text-gray-400 font-medium"
              >Nome da empresa</span
            >
            <input
              type="text"
              class="pt-6 pb-3 px-4 w-[570px] rounded-md"
              placeholder="Qual o nome da sua empresa?"
            />
          </label>
          <label class="relative" for="">
            <span class="absolute py-2 px-4 text-xs text-gray-400 font-medium"
              >Instagram da empresa</span
            >
            <input
              type="text"
              class="pt-6 pb-3 px-4 w-[570px] rounded-md"
              placeholder="Informe o @perfil de sua empresa"
            />
          </label>
          <label class="relative" for="">
            <span class="absolute py-2 px-4 text-xs text-gray-400 font-medium"
              >Qual o ramo do seu negócio</span
            >
            <input
              type="text"
              class="pt-6 pb-3 px-4 w-[570px] rounded-md"
              placeholder="Em que àrea sua empresa atua?"
            />
          </label>
          <label class="relative" for="">
            <span class="absolute py-2 px-4 text-xs text-gray-400 font-medium"
              >Quantidade de funcionários</span
            >
            <input
              type="text"
              class="pt-6 pb-3 px-4 w-[570px] rounded-md"
              placeholder="Quantas pessoas trabalham com você"
            />
          </label>
          <label class="relative" for="">
            <span class="absolute py-2 px-4 text-xs text-gray-400 font-medium"
              >Escreva-nos uma mensagem</span
            >
            <textarea
              type="text"
              class="pt-6 pb-3 px-4 w-[570px] rounded-md"
              placeholder="Faça alguma observação ou deixe uma mensagem para nós"
            />
          </label>
          <button
            type="submit"
            class="bg-[#F2632D] px-16 pt-3 pb-4 rounded-full font-title text-white w-max uppercase text-[20px]"
          >
            Enviar
          </button>
        </form>
      </div>
    </div>
  </div>
</template>

<style lang="postcss" scoped>
.gradient-text {
  background: linear-gradient(
    90deg,
    #f2a01e 3.44%,
    #f29c20 25.23%,
    #f19126 47.02%,
    #f07e30 66.51%,
    #ef633e 87.15%,
    #ed4251 105.5%,
    #ec305a 114.68%
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  text-fill-color: transparent;
}

form label {
  & input:focus {
    @apply bg-gray-100;
  }
}
</style>
