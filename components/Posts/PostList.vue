<template>
  <section class="post-list">
    <PostPreview
      id="1"
      title="Hello there!"
      previewText="This is my first post!"
      thumbnailUrl="https://www.bworldonline.com/wp-content/uploads/2018/03/Powerful-Tech.jpg"
    />
    <PostPreview
      id="2"
      title="Hello there - this is my second post!"
      previewText="This is my second post!"
      thumbnailUrl="https://www.bworldonline.com/wp-content/uploads/2018/03/Powerful-Tech.jpg"
    />
    <PostPreview
      id="3"
      title="I love You Phuong Thao"
      previewText="This is my third post!"
      thumbnailUrl="https://www.bworldonline.com/wp-content/uploads/2018/03/Powerful-Tech.jpg"
    />
  </section>
</template>

<script>
import PostPreview from "@/components/Posts/PostPreview";

export default {
  name: "PostList",
  components: {
    PostPreview,
  },
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