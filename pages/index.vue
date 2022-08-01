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

      <!-- statuses skeletons (loading placeholder / loading indicator) -->
      <template v-if="loading">
        <IndexStatusSkeleton />
        <IndexStatusSkeleton />
        <IndexStatusSkeleton />
      </template>

      <!-- stasuses -->
      <template v-else>
        <IndexStatus
          v-for="(post, index) in posts"
          :key="'post-' + post.id + index"
          :post="post"
        />
      </template>
    </section>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      loading: false,
      posts: [],
    }
  },
  async fetch() {
    await this.getPosts()
  },
  methods: {
    async getPosts() {
      this.loading = true

      try {
        const res = await this.$axios.get(
          'https://jsonplaceholder.typicode.com/posts'
        )

        // console.log('getPosts res.data', res.data)

        this.posts = res.data
      } catch {
        // show err popup
      }

      this.loading = false
    },
  },
}
</script>
