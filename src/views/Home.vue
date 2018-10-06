<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <TodoMain msg="Welcome to the Todo App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import TodoMain from '@/components/TodoMain.vue'

export default {
  name: 'home',
  components: {
    TodoMain
  }
}
</script>
