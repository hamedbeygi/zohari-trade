<template>
  <button :class="mode" v-on="$listeners">
    <slot></slot>
  </button>
</template>

<script>
export default {
  props: ["mode"],
};
</script>

<style scoped>
button {
  font-family: inherit;
  padding: 0.7em;
  border: none;
  margin: 0.3em;
  cursor: pointer;
  border-radius: 0.3em;
}
.primary {
  background-color: var(--second);
  color: var(--sixth);
}
.primary:hover {
  background-color: var(--sixth);
  color: var(--second);
}
.secondary {
  background-color: var(--sixth);
  color: var(--second);
}
.secondary:hover {
  background-color: var(--second);
  color: var(--sixth);
}
</style>
