<template>
  <div>
      <Header />
      <todo-app-list>
       <todo-item v-for="i in 5" :key="i" :index="i" />
      </todo-app-list>
  </div>
</template>

<script>
import TodoAppList from '../components/Todo-app-list'
import TodoItem from '../components/Todo-item'
import Header from '../components/Header'
export default {
  head() {
    return {
      title: 'To Do List'
    }
  },
  components: {
    TodoAppList,
    TodoItem,
    Header
  }
}
</script>

