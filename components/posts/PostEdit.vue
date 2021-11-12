<template>
  <div>
    <client-only>
      <VueEditor v-model="content" @input="dothis" class="editor" />
    </client-only>
    <p v-html="content"></p>
    <base-button mode="primary" @click="$emit('save', content)"
      >Save</base-button
    >
    <base-button mode="primary" @click="$emit('cancel')">Cancel</base-button>
  </div>
</template>

<script>
import BaseButton from "~/components/UI/BaseButton";
const myEditor = () => import("vue2-editor");
export default {
  props: ["value"],
  components: {
    myEditor,
    BaseButton,
  },
  data() {
    return {
      content: this.value,
    };
  },
  methods: {
    dothis() {
      console.log(this.content);
    },
  },
};
</script>
<style scoped>
.editor {
  background-color: var(--sixth);
  color: black;
  cursor: pointer;
}
</style>
