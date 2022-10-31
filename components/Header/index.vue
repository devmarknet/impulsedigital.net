<script lang="ts">
import Vue, { PropOptions } from 'vue'

interface HeaderData {
  title: string
  body: string
  actionUrl: string
  actionTitle: string
  image: string
}

export default Vue.extend({
  name: 'HeaderComponent',
  props: {
    data: {
      type: Object,
      required: true,
    } as PropOptions<HeaderData>,
  },
})
</script>

<template>
  <header
    class="flex items-center justify-center h-screen"
    :style="`background: url(${require('~/assets/images/header-bg.png')})`"
  >
    <div class="container mx-auto">
      <div class="flex items-center justify-between w-full relative">
        <div class="flex flex-col gap-8">
          <h1
            class="text-white font-title font-bold uppercase text-[60px] leading-[72px] max-w-[848px]"
          >
            {{ data.title }}
          </h1>
          <p
            class="text-white/70 font-light text-[38px] leading-[48px] max-w-[720px]"
          >
            {{ data.body }}
          </p>
          <a
            class="bg-[#F2632D] text-white py-4 px-10 w-max rounded-full uppercase text-sm"
            :href="data.actionUrl"
            >{{ data.actionTitle }}</a
          >
        </div>
        <img
          class="xl:[60%]"
          width="auto"
          height="auto"
          :src="require(`~/assets/svg/${data.image}`)"
          alt="Asset Header"
        />
      </div>
    </div>
  </header>
</template>
