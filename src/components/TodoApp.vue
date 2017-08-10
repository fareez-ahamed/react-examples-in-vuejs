<template>
<div>
  <h3>TODO</h3>
  <todo-list :items="items" />
  <form @submit.prevent="handleSubmit">
    <input v-model="text" />
    <button>{{ 'Add ' + (items.length + 1) }}</button>
  </form>
</div>
</template>
<script>
import TodoList from './TodoList'

export default {

  components: { TodoList },

  data () {
    return {
      items: [],
      text: ''
    }
  },

  methods: {
    handleSubmit () {
      var newItem = {
        text: this.text,
        id: Date.now()
      }
      this.items.push(newItem)
      this.text = ''
    }
  }
}
</script>
