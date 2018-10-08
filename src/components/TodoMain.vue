<template>
  <div class="hello">
    <h2>{{ msg }}</h2>
      <div v-for="todo in todos" v-bind:key="todo.id">
        <router-link to="/editTodos">
          <h4>
            {{ todo.name }} -
              <span class="completed" v-if="todo.completed">completed</span>
              <span class="not-completed" v-else>not completed</span>
          </h4>
        </router-link>
      </div>
  </div>
</template>

<script>
export default {
  name: 'TodoMain',
  props: {
    msg: String
  },
  data() {
    return {
      todos: [
        { name: "master vue", completed: false },
        { name: "master node", completed: false }
      ]
    }
  },
}
</script>

<style>
  .completed {
      color: green;
  }
  .not-completed {
      color: red;
  }
</style>


<!-- Add "scoped" attribute to limit CSS to this component only -->
