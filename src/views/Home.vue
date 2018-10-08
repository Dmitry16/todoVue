<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <h3>{{ msg }}</h3>
    <TodoMain msg="All Todos:"/>
  </div>
</template>

<script>
// @ is an alias to /src
import TodoMain from '@/components/TodoMain.vue'

export default {
  name: 'home',
    data() {
      return {
          todos: [
              { name: "master vue", completed: false },
              { name: "master node", completed: false }
          ],
          msg: "Wellcome to the awsome Todo App!"
      }
    },
  components: {
    TodoMain
  }
}
</script>
