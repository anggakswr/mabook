<template>
  <nav class="flex gap-x-[10px] justify-end">
    <NuxtLink
      to="#"
      class="h-[40px] w-[40px] rounded-full bg-gray-600 box-center"
    >
      <client-only>
        <unicon name="list-ul" fill="white" />
      </client-only>
    </NuxtLink>

    <NuxtLink
      to="#"
      class="h-[40px] w-[40px] rounded-full bg-gray-600 box-center"
    >
      <client-only>
        <unicon name="comment" fill="white" />
      </client-only>
    </NuxtLink>

    <NuxtLink
      to="#"
      class="h-[40px] w-[40px] rounded-full bg-gray-600 box-center"
    >
      <client-only>
        <unicon name="bell" fill="white" />
      </client-only>
    </NuxtLink>

    <NuxtLink
      to="#"
      class="h-[40px] w-[40px] rounded-full"
      :style="{ backgroundImage: 'url(https://picsum.photos/40)' }"
    />
  </nav>
</template>

<script>
export default {}
</script>
