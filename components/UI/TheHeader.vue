<template>
  <div class="theheader">
    <div>
      <nuxt-link to="/"><h2>zohari trade</h2></nuxt-link>
    </div>
    <div>
      <nuxt-link to="/about"
        ><base-button mode="primary">About Us</base-button></nuxt-link
      >
      <nuxt-link to="/contact"
        ><base-button mode="primary">Contact Us</base-button>
      </nuxt-link>
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
.theheader {
  display: flex;
  align-items: center;
  justify-content: space-around;
  background-color: #2e3335;
}
a {
  text-decoration: none;
  color: var(--sixth);
}
</style>
