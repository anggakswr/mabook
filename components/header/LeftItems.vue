<template>
  <nav class="box-equal gap-x-[10px]">
    <NuxtLink
      to="/"
      class="h-[40px] w-[40px] min-h-[40px] min-w-[40px] max-h-[40px] max-w-[40px] rounded-full text-[20px] box-center bg-gradient-to-b from-indigo-500 font-bold"
    >
      M
    </NuxtLink>

    <div class="relative">
      <div class="absolute left-[10px] inset-y-0 box-center">
        <client-only>
          <unicon name="search" fill="white" width="20px" />
        </client-only>
      </div>

      <input
        type="text"
        class="bg-gray-600 rounded-full h-[40px] p-[10px] pl-[40px] focus:outline-none w-full"
        placeholder="Cari di Mabook"
      />
    </div>
  </nav>
</template>

<script>
export default {}
</script>
