<template>
  <nav class="fixed w-1/4 right-0 top-[70px] bottom-0 overflow-y-scroll">
    <h2 class="font-bold mb-4 text-xl">Bersponsor</h2>

    <RightNavSponsor />
    <RightNavSponsor />

    <hr class="border-t border-gray-700 mb-4" />

    <RightNavKontakHeader />

    <!-- chats -->
    <RightNavPerson v-for="number in 10" :key="'person-' + number" />
  </nav>
</template>

<script>
export default {}
</script>
