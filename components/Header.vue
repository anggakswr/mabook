<template>
  <!-- <nav
    class="bg-gray-700 border-b border-gray-500 fixed inset-x-0 top-0 box-between text-white px-[10px] py-[5px]"
  > -->
  <nav
    class="bg-gray-700 border-b border-gray-500 fixed inset-x-0 top-0 text-white px-[10px] py-[5px] grid grid-cols-4 gap-x-[20px]"
  >
    <!-- img & search box -->
    <HeaderLeftItems class="col-span-1" />

    <!-- btns -->
    <HeaderCenterItems class="col-span-2" />

    <!-- btns -->
    <div class="col-span-1">asd</div>
  </nav>
</template>

<script>
export default {
  name: 'DefaultHeader',
}
</script>
