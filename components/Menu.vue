<template>
  <ul>
    <li><h4>Menu item</h4></li>
    <li><h4>Menu item</h4></li>
    <li><h4>Menu item</h4></li>
    <li><h4>Menu item</h4></li>
    <li><h4>Menu item</h4></li>
    <li><h4>Menu item</h4></li>
    <li><h4>Menu item</h4></li>
    <li><h4>Menu item</h4></li>
  </ul>
</template>

<style scoped>
ul {
  margin: 0;
  padding: 0;
}
li {
  cursor: pointer;
  display: flex;
  list-style: none;
  padding: 0.8em 0;
  border-bottom: 2px var(--third) solid;
}
li:hover {
  background-color: var(--third);
  color: var(--first);
}
h4 {
  margin: 0 auto 0 0.5em;
  font-weight: lighter;
}
</style>
