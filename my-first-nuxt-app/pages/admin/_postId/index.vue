<template>
    <div class="admin-post-page">
        <section class="update-form">
            <AdminPostForm :post="loadedPost" />
        </section>
    </div>
</template>

<script lang="ts">
import Vue from 'vue'
import AdminPostForm from '@/components/Admin/AdminPostForm'
export default {
    layout: 'admin',
    components: { AdminPostForm },
    data(){
        return{
            loadedPost: {
                author: 'Thiago',
                title: 'My awesome Post',
                content: 'Super amazing, thanks for that!',
                thumbnailLink: 'https://cdn.gamer-network.net/2015/articles/1/8/4/8/0/4/5/the-witcher-3-fine-art-prints-are-gorgeous-indeed-1470320516485.jpg/EG11/thumbnail/1920x1278/format/jpg/quality/80'
            }
        }
    }
}
</script>

<style scoped>
.update-form {
  width: 90%;
  margin: 20px auto;
}
@media (min-width: 768px) {
  .update-form {
    width: 500px;
  }
}
</style>