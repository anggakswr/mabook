<template>
  <main class="bg-gray-900 min-h-screen text-white">
    <Header />

    <!-- page -->
    <section class="grid grid-cols-4 pt-[70px]">
      <div class="col-span-1">asd</div>
      <Nuxt class="col-span-2 px-[40px]" />
      <div class="col-span-1">asd</div>
    </section>

    <!-- snackbar in left bottom -->
    <Snackbar />
  </main>
</template>

<script>
export default {
  name: 'GroupsLayout',
}
</script>
