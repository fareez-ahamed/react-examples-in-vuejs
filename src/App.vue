<template>
  <div class="container">
    <section class="section">
      <h1 class="title">Hello World</h1>
      <hello name="Ahamed"></hello>
    </section>
    <section class="section">
      <h1 class="title">Timer</h1>
      <timer></timer>
    </section>
    <section class="section">
      <h1 class="title">Todo App</h1>
      <todo-app></todo-app>
    </section>
    <section class="section">
      <h1 class="title">Markdown Editor</h1>
      <markdown-editor></markdown-editor>
    </section>
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
