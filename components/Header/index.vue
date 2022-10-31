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
  <header class="flex items-center justify-center overflow-hidden">
    <div class="container mx-auto">
      <div class="content">
        <div class="flex flex-col justify-between p-6 gap-6 z-10">
          <h1
            class="text-3xl xl:text-6xl text-white uppercase font-title font-bold"
          >
            {{ data.title }}
          </h1>
          <p class="text-white font-light text-xl">{{ data.body }}</p>
          <a
            class="bg-[#F2632D] text-white py-4 px-10 w-max rounded-full uppercase text-sm"
            :href="data.actionUrl"
            >{{ data.actionTitle }}</a
          >
        </div>
        <img
          class="w-full -mt-10 -z-10"
          width="auto"
          height="auto"
          :src="require(`~/assets/svg/${data.image}`)"
          alt="Asset Header"
        />
      </div>
    </div>
  </header>
</template>
