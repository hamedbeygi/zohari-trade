<template>
  <div class="item" @click="$emit('clicked')">
    <img src="@/assets/pic.jpg" alt="pic" />
    <slot name="header"></slot>
    <slot name="desc"></slot>
  </div>
</template>

<style scoped>
img {
  height: auto;
  max-width: 100%;
  border-radius: 0.2em;
}
.item {
  border: 2px solid rgb(80, 80, 80);
  list-style: none;
  clear: both;
  text-align: center;
  cursor: pointer;
  margin: 0 0.5em 0.5em 0;
  border-radius: 0.2em;
}
</style>
