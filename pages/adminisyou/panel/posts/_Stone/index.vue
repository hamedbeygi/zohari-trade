<template>
  <div>
    <PostEdit @cancel="cancel" @save="doSave" />
  </div>
</template>

<script>
import PostEdit from "~/components/posts/PostEdit.vue";
import axios from "axios";
export default {
  components: {
    PostEdit,
  },
  layout: "panel",
  methods: {
    doSave(content) {
      axios
        .post("https://nuxt-one-2f33d-default-rtdb.firebaseio.com/posts.json", {
          content,
        })
        .then((res) => console.log(res))
        .catch((e) => console.log(e));
    },
    cancel() {
      this.$router.back();
    },
  },
};
</script>
<style scoped></style>
