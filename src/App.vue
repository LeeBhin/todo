<template>
  <v-app>
    <v-container>
      <v-row>
        <v-col>
          <router-view/>
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<script>
import AddTodo from './components/AddTodo.vue';
import ToDoList from './components/ToDoList.vue';

export default {
  name: 'App'
}
</script>