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
  <!-- <header
    class="flex items-center justify-center h-screen"
    :style="`background: url(${require('~/assets/images/header-bg.png')})`"
  > -->
  <header class="flex items-center justify-center">
    <div class="container mx-auto px-6">
      <div class="flex items-center justify-between w-full relative flex-col md:flex-row">
        <div class="flex flex-col gap-8">
          <h1 class="title max-w-[848px]">
            {{ data.title }}
          </h1>
          <p class="text-cover max-w-[720px]">
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
