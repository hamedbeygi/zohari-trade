<template>
  <div>
    <div class="list">
      <stone-item>
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
      <stone-item>
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
      <stone-item>
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
    <div class="list">
      <stone-item>
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
      <stone-item>
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
      <stone-item>
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
    <div class="list">
      <stone-item>
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
      <stone-item>
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
      <stone-item>
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
  </div>
</template>

<script>
import StoneItem from "@/components/StoneItem";
export default {
  components: { StoneItem },
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
