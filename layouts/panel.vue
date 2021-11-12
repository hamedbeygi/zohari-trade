<template>
  <div>
    <div class="header">
      <div>
        <nuxt-link to="/"><h2>zohari trade</h2></nuxt-link>
      </div>
      <div>
        <nuxt-link to="/adminisyou/panel/posts/newpost"
          ><base-button mode="primary">Add Post</base-button></nuxt-link
        >
        <nuxt-link to="/adminisyou/panel/messages"
          ><base-button mode="primary">Messages</base-button>
        </nuxt-link>
      </div>
    </div>
    <div class="content">
      <nuxt />
    </div>
  </div>
</template>

<script>
import BaseButton from "~/components/UI/BaseButton";
export default {
  components: { BaseButton },
};
</script>

<style scoped>
.header {
  display: flex;
  align-items: center;
  justify-content: space-around;
  background-color: #2e3335;
}
a {
  text-decoration: none;
  color: var(--sixth);
}
.content {
  margin: 3em auto;
  border-radius: 1em;
  width: 65%;
  padding: 2em;
  background-color: #363a3d;
}
</style>
