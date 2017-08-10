<template>
  <div class="container">
    <hello name="Ahamed"></hello>
    <timer></timer>
    <todo-app></todo-app>
    <markdown-editor></markdown-editor>
  </div>
</template>

<script>
import Hello from './components/Hello'
import Timer from './components/Timer'
import TodoApp from './components/TodoApp'
import MarkdownEditor from './components/MarkdownEditor'

export default {
  name: 'app',
  components: {
    Hello, Timer, TodoApp, MarkdownEditor
  }
}
</script>

<style lang="sass">
@import '../node_modules/bulma/bulma.sass'
</style>
