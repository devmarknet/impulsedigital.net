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
  <main class="flex flex-col">
    <Navbar />
    <Header :data="header" class="pt-16 pb-32" />
    <About class="py-32" />
    <Services class="py-32" />
    <Inovation class="pt-64 pb-32" />
    <WebsitesDevelopment class="pt-32 pb-2" />
    <Jobs class="pt-24 pb-32" />
    <Integration class="py-32" />
    <Enterprise class="py-32" />
    <Form />
  </main>
</template>

<style>
body {
  background: url('../assets/images/bg-splash.png');
}
</style>
