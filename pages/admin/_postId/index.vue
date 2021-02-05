<template>
  <div class="admin-post-page">
    <section class="update-form">
      <AdminPostForm :post="loadedPost" />
    </section>
  </div>
</template>

<script>
import AdminPostForm from "@/components/Admin/AdminPostForm";

export default {
  components: {
    AdminPostForm,
  },
  data() {
    return {
      loadedPost: {
        author: "Hoang",
        title: "My post",
        content: "superman",
        thumbnailLink:
          "https://cdn-images-1.medium.com/max/1024/1*dzkwVxqR90VdYw_pnzuZUg.jpeg",
      },
    };
  },
};
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