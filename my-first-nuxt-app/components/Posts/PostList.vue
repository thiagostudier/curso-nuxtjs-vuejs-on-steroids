<template>
    <section class="post-list">
      <PostPreview id="1" :is-admin="isAdmin" title="Hello there! First Post" thumbnail="https://cdn.gamer-network.net/2015/articles/1/8/4/8/0/4/5/the-witcher-3-fine-art-prints-are-gorgeous-indeed-1470320516485.jpg/EG11/thumbnail/1920x1278/format/jpg/quality/80" previewText="This my first post"/>
      <PostPreview id="1" :is-admin="isAdmin" title="Hello there! Second Post" thumbnail="https://cdn.gamer-network.net/2015/articles/1/8/4/8/0/4/5/the-witcher-3-fine-art-prints-are-gorgeous-indeed-1470320516485.jpg/EG11/thumbnail/1920x1278/format/jpg/quality/80" previewText="This my first post"/>
      <PostPreview id="1" :is-admin="isAdmin" title="Hello there! Thirth Post" thumbnail="https://cdn.gamer-network.net/2015/articles/1/8/4/8/0/4/5/the-witcher-3-fine-art-prints-are-gorgeous-indeed-1470320516485.jpg/EG11/thumbnail/1920x1278/format/jpg/quality/80" previewText="This my first post"/>
    </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'
export default {
    name: 'PostList',
    components: {PostPreview},
    props: {
        isAdmin: {
            type: Boolean,
            default: false
        }
    }
};
</script>

<style scoped>
.post-list {
    display: flex;
    padding: 20px;
    box-sizing: border-box;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
}
</style>