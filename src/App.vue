<template>
  <nav class="navbar navbar-light bg-light">
    <a class="navbar-brand" href="#">VueJS Todolist</a>
  </nav>
  <div class="container">
    <AddTodoItem />
  </div>
</template>

<script>
import AddTodoItem from './components/AddTodoItem.vue';

export default {
    name: "App",
    data() {
        return {
            todoItems: [
                {
                    title: "FirstItem",
                    done: false,
                    deadline: Date()
                }
            ]
        };
    },
    components: { AddTodoItem }
}
</script>