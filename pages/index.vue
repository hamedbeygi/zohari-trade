<template>
  <div>
    <the-header></the-header>
    <div class="container">
      <div class="left">
        <Menu />
      </div>
      <div class="right"><router-view /></div>
    </div>
  </div>
</template>

<script>
import TheHeader from "@/components/TheHeader.vue";
import Menu from "@/components/Menu.vue";
export default {
  components: { TheHeader, Menu },
};
</script>
``

<style>
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap");

:root {
  --first: #1e2019;
  --second: #393e41;
  --third: #e2c044;
  --forth: #587b7f;
  --fifth: #e9724c;
  --sixth: #d3d0c8;
}
html {
  font-family: "Roboto", sans-serif;
}
.container {
  display: flex;
  margin: 0 1em;
}
.left {
  position: relative;
  left: 1em;
  width: 15%;
  padding: 2em;
  background-color: #363a3d;
}
.right {
  position: absolute;
  right: 2em;
  width: 70%;
  padding: 2em;
  background-color: #363a3d;
}
body {
  background-color: var(--second);
  color: var(--sixth);
  margin: 0;
}

::-webkit-scrollbar {
  width: 5px;
}
::-webkit-scrollbar-thumb {
  background-color: #808080;
}
</style>
