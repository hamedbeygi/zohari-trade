<template>
  <div class="contain">
    <form @submit.prevent="">
      <div class="c2">
        <label for="email">Email</label>
        <input type="text" id="email" />
      </div>
      <div class="c2">
        <label for="password">Password</label>
        <input type="password" id="password" />
      </div>
      <base-button mode="secondary">Login</base-button>
    </form>
  </div>
</template>

<script>
import BaseButton from "~/components/UI/BaseButton";
export default {
  components: { BaseButton },
  layout: "admin",
};
</script>

<style scoped>
.contain {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 40vh;
}
form {
  padding: 2em;
  border: 1px var(--sixth) solid;
  border-radius: 0.5em;
}
.c2 {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1em;
}
label {
  padding: 0 1em;
}
input {
  border: none;
  background-color: var(--sixth);
  padding: 0.5em;
  border-radius: 1em;
}
</style>
