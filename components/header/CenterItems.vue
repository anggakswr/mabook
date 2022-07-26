<template>
  <nav class="grid grid-cols-5 gap-x-[5px]">
    <NuxtLink
      v-for="link in links"
      :key="link.icon"
      :to="link.url"
      class="box-center hover:bg-gray-600 rounded-lg"
    >
      <client-only>
        <unicon
          :name="link.icon"
          :fill="$route.path === link.url ? '#9400FF' : 'white'"
        />
      </client-only>
    </NuxtLink>
  </nav>
</template>

<script>
const links = [
  { url: '/', icon: 'estate' },
  { url: '#', icon: 'video' },
  { url: '#', icon: 'store' },
  { url: '#', icon: 'users-alt' },
  { url: '#', icon: 'basketball' },
]

export default {
  data() {
    return {
      links,
    }
  },
}
</script>

<style scoped>
a.nuxt-link-exact-active {
  @apply border-b-2 border-purple-500 rounded-none hover:bg-gray-700;
}
</style>
