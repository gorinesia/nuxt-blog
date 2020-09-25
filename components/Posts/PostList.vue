<template>
  <section class="post-list">
      <PostPreview 
        id="1"
        :is-admin="isAdmin"
        thumbnail="http://4.bp.blogspot.com/-kBsKTbWxCRQ/T9TRVCRGqoI/AAAAAAAAKRQ/ESK-JCzJiWM/s1600/[wallcoo_com]_3528_future_TECH_Image.jpg"
        title="Hello there!"
        previewText="This my first post!" />
      <PostPreview 
        id="2"
        :is-admin="isAdmin"
        thumbnail="http://4.bp.blogspot.com/-kBsKTbWxCRQ/T9TRVCRGqoI/AAAAAAAAKRQ/ESK-JCzJiWM/s1600/[wallcoo_com]_3528_future_TECH_Image.jpg"
        title="Hello there - the second time!"
        previewText="This my second post!" />
      <PostPreview 
        id="3"
        :is-admin="isAdmin"
        thumbnail="http://4.bp.blogspot.com/-kBsKTbWxCRQ/T9TRVCRGqoI/AAAAAAAAKRQ/ESK-JCzJiWM/s1600/[wallcoo_com]_3528_future_TECH_Image.jpg"
        title="Hello there - the third time!"
        previewText="This my third post!" />
    </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'

export default {
  components: {
    PostPreview
  },
  props: {
    isAdmin: {
      type: Boolean,
      default: false
    }
  }
}
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