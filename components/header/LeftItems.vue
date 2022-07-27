<template>
  <nav class="box-equal gap-x-[10px]">
    <NuxtLink
      to="/"
      class="h-[40px] w-[40px] min-h-[40px] min-w-[40px] max-h-[40px] max-w-[40px] rounded-full text-[20px] bg-gradient-to-b from-indigo-500 to-blue-500 font-bold relative overflow-hidden"
    >
      <span
        class="absolute -bottom-[5px] inset-x-0 flex justify-center text-3xl"
      >
        M
      </span>
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
