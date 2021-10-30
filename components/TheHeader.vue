<template>
  <div class="theheader">
    <div>
      <router-link to="/"><h2>zohari trade</h2></router-link>
    </div>
    <div>
      <router-link to="/about"
        ><base-button mode="primary">About Us</base-button></router-link
      >
      <router-link to="/contact"
        ><base-button mode="primary">Contact Us</base-button>
      </router-link>
    </div>
  </div>
</template>

<style scoped>
div {
  display: flex;
  align-items: center;
  justify-content: space-around;
}
.theheader {
  background-color: #2e3335;
}

a {
  text-decoration: none;
  color: var(--sixth);
}
</style>
