<template>
    <div>
      <input v-model="newTodo" placeholder="Add a new to-do" @keyup.enter="submitTodo" />
      <button @click="submitTodo">Add</button>
    </div>
  </template>
  
  <script>
  export default {
    name: 'AddTodo',
    data() {
      return {
        newTodo: ''
      };
    },
    methods: {
      submitTodo() {
        if (this.newTodo.trim()) {
          this.$emit("add-todo", this.newTodo);
          this.newTodo = '';
        }
      }
    }
  };
  </script>
  