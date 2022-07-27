<template>
  <main class="bg-gray-900 min-h-screen text-white">
    <Header />

    <div class="grid grid-cols-4 pt-[70px] gap-x-[20px]">
      <LeftSideNav class="col-span-1" />
      <Nuxt class="col-span-2" />
      <!-- <RightSideNav class="col-span-1" /> -->
    </div>
  </main>
</template>

<script>
export default {
  name: 'DefaultLayout',
}
</script>
