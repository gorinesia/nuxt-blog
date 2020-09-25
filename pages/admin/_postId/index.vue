<template>
  <div class="admin-post-page">
    <section class="update-form">
      <AdminPostForm :post="loadedPost" />
    </section>
  </div>
</template>

<script>
import AdminPostForm from '@/components/Admin/AdminPostForm'

export default {
  layout: 'admin',
  components: {
    AdminPostForm
  },
  data() {
    return {
      loadedPost: {
        author: 'Akinori',
        title: 'My awesome Post',
        content: 'Super amazing thanks for that!',
        thumbnailLink: 'http://4.bp.blogspot.com/-kBsKTbWxCRQ/T9TRVCRGqoI/AAAAAAAAKRQ/ESK-JCzJiWM/s1600/[wallcoo_com]_3528_future_TECH_Image.jpg'
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