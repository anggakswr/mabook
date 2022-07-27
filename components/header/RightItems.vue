<template>
  <nav class="flex gap-x-[10px] justify-end">
    <NuxtLink
      v-for="link in links"
      :key="'right-item-' + link.icon"
      :to="link.url"
      class="h-[40px] w-[40px] rounded-full bg-gray-600 hover:bg-gray-500 box-center"
    >
      <client-only>
        <unicon :name="link.icon" fill="white" />
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
const links = [
  { url: '#', icon: 'list-ul' },
  { url: '#', icon: 'comment' },
  { url: '#', icon: 'bell' },
]

export default {
  data() {
    return {
      links,
    }
  },
}
</script>
