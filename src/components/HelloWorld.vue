<template>
  <MonacoEditor class="editor" v-model="code" language="javascript" />
</template>

<script>
import MonacoEditor from 'vue-monaco'

export default {
  components: {
    MonacoEditor
  },

  data() {
    return {
      code: 'const noop = () => {}'
    }
  }
}
</script>

<style>
.editor {
  width: 1600px;
  height: 800px;
}
</style>
