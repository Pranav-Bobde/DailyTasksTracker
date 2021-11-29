<template>
  <q-list
    class="rounded-borders"
    bordered
    separator
  >
      <q-item-label header>Daily Tasks</q-item-label>

      <q-item v-for="todo in todos" :key="todo.index">
        <q-item-section class="col-1">
          <q-item-label class="text-h4 text-center" >{{todo.index}}</q-item-label>
        </q-item-section>

        <q-item-section class="col-2 text-center">
          <q-item-label class="q-mt-sm text-body1 ">{{todo.title}}</q-item-label>
        </q-item-section>

        <q-item-section >
          <q-item-label lines="2">
            <span class="text-body1">{{todo.desc}}</span>
          </q-item-label>
        </q-item-section>

        <q-item-section top side>
          <div class="text-grey-8 q-gutter-xs">
            <q-btn class="gt-xs" size="12px" flat dense round icon="delete" />
            <q-btn class="gt-xs" size="12px" flat dense round icon="done" />
            <q-btn size="12px" flat dense round icon="more_vert" />
          </div>
        </q-item-section>
      </q-item>
    </q-list>
</template>

<script>
export default {
  name: 'TodoTask',
  data() {
    return {
      todos: [
        {
          index: '1',
          title: 'DBMS Vids',
          desc: 'Watch DBMS YT Vid',
        },
        {
          index: '2',
          title: 'CN Vids',
          desc: 'Watch CN YT Vid',
        }
      ]
    }
  },
  
}
</script>
