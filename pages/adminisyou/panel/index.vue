<template>
  <div>
    <Posts @clicked="show" />
  </div>
</template>

<script>
import Posts from "~/components/posts/Posts.vue";
export default {
  components: {
    Posts,
  },
  layout: "panel",
  methods: {
    show() {
      this.$router.push("/adminisyou/panel/posts/1");
    },
  },
};
</script>

<style scoped></style>
