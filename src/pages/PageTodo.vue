<template>
  <q-page>
    <TodoTask />
  </q-page>
</template>

<script>
import TodoTask from 'components/TodoTask.vue'
export default {
  name: 'PageTodo',
  components:{
    TodoTask
  }
}
</script>
