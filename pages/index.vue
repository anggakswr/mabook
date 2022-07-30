<template>
  <div>
    <!-- stories -->
    <IndexStories />

    <section class="px-[30px]">
      <div class="rounded-lg bg-gray-700 p-[10px] mb-[20px]">
        <!-- input box (to create new status) -->
        <IndexInputBox />

        <!-- video btn & img btn -->
        <IndexBtns />
      </div>

      <!-- stasuses -->
      <IndexStatus />
      <IndexStatus />
      <IndexStatus />
    </section>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>
