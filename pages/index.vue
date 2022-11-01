<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage',
  async asyncData({ $content }): Promise<any> {
    const header = await $content('header').fetch()
    return { header }
  },
})
</script>

<template>
  <main class="flex flex-col gap-64">
    <Header :data="header" />
    <About />
    <Services />
    <Inovation />
    <WebsitesDevelopment />
    <Jobs />
    <Integration />
    <Enterprise />
  </main>
</template>
