<template>
  <main class="bg-gray-900 min-h-screen text-white">
    <Header />

    <LeftNav />
    <section class="grid grid-cols-4 pt-[70px]">
      <div class="col-span-1" />
      <Nuxt class="col-span-2 px-[20px]" />
      <div class="col-span-1" />
    </section>
    <RightNav />
  </main>
</template>

<script>
export default {
  name: 'DefaultLayout',
}
</script>
