<template>
    <div class="posts-page">
        <PostList />
    </div>
</template>

<script lang="ts">
import PostList from '@/components/Posts/PostList'
export default {
  components: {
    PostList
  }
}
</script>

<style scoped>
.posts-page{
    display: flex;
    justify-content: center;
    align-items: center;
}
</style>