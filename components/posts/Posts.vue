<template>
  <div>
    <div class="list">
      <stone-item @clicked="$emit('clicked')">
        <template v-slot:header>
          <h2>Best Stone</h2>
        </template>
        <template v-slot:desc>
          <h4>
            This is just a short description in order <br />
            test how the content would view in the list
          </h4>
        </template>
      </stone-item>
    </div>
    <p v-html="data"></p>
  </div>
</template>

<script>
import StoneItem from "@/components/StoneItem";
import axios from "axios";
export default {
  components: { StoneItem },
  data() {
    return {
      data: "",
    };
  },
  created() {
    axios
      .get("https://nuxt-one-2f33d-default-rtdb.firebaseio.com/posts.json")
      .then((res) => {
        const postArray = [];
        for (const key in res.data) {
          postArray.push(res.data[key].content);
        }
        this.data = postArray;
        console.log(this.data);
      })
      .catch((e) => console.log(e));
  },
};
</script>

<style scoped>
h2,
h4 {
  margin-top: 0.6em;
  font-family: inherit;
  font-weight: lighter;
}
.list {
  word-wrap: break-word;
  margin-left: 4em;
  display: flex;
}
</style>
