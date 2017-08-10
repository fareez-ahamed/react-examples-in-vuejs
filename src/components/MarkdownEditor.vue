<template>
<div>
  <h3>Input</h3>
  <textarea v-model="text" />
  <h3>Output</h3>
  <div v-html="markdownText"></div>
</div>
</template>
<script>
let Remarkable = require('remarkable')
let md = new Remarkable()

export default {

  data () {
    return {
      text: ''
    }
  },

  computed: {
    markdownText () {
      return md.render(this.text)
    }
  }

}
</script>
