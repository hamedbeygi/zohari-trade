<template>
  <button :class="mode">
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
  background-color: var(--second);
  color: var(--sixth);
  font-family: inherit;
  padding: 0.7em;
  border: none;
  margin: 0.3em;
  cursor: pointer;
  border-radius: 0.3em;
}
button:hover {
  background-color: var(--sixth);
  color: var(--second);
}
</style>
