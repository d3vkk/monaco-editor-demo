<template>
  <div id="app">
    <MonacoEditor class="editor" v-model="code" language="javascript" />
  </div>
</template>

<script>
import MonacoEditor from "vue-monaco";

export default {
  name: "App",
  components: {
    MonacoEditor,
  },
  data() {
    return {
      code: "console.log('Hello World!')",
    };
  },
};
</script>

<style>
.editor {
  width: 1000px;
  height: 800px;
}
</style>
