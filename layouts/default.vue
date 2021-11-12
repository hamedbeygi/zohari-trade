<template>
  <div>
    <TheHeader />
    <div class="container">
      <div class="left">
        <Menu />
      </div>
      <div class="right"><nuxt /></div>
    </div>
  </div>
</template>

<script>
import TheHeader from "~/components/UI/TheHeader";
export default {
  components: { TheHeader },
};
</script>

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
  margin: 3em 1em;
}
.left {
  border-radius: 1em;
  position: relative;
  left: 2em;
  width: 15%;
  padding: 2em;
  background-color: #363a3d;
  padding-bottom: 10em;
}
.right {
  border-radius: 1em;
  position: absolute;
  right: 5em;
  width: 65%;
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
