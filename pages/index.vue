<template>
  <article class="pa3 pa5-ns">
    <h1 class="f4 bold center mw6">Todos</h1>
    <ul class="list pl0 ml0 center mw6 ba b--light-silver br2">
      <li v-for="todo in todos" :key="todo.task" class="ph3 pv3 bb b--light-silver">{{todo.task}}</li>
    </ul>
  </article>
</template>

<script>
import { mapState, mapMutations } from "vuex";

export default {
  computed: {
    ...mapState({
      todos: state => state.todos
    })
  },

  methods: {}
};
</script>


<style>
h1 {
  font-family: Roboto, sans-serif;
}
</style>
