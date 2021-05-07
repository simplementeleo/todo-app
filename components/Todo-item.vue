<template>
  <div class="p-5 flex items-center todo-item text-gray-500 relative">
    <div class="absolute top-0 right-0 settings flex items-center h-full">
      <i class="fa fa-times text-red-700 text-xl p-3 cursor-pointer h-full w-16 flex items-center justify-center"></i>
    </div>
    <div class="completed relative">
     
    </div>
    <div>
      Tarea {{ index }}
    </div>
  </div>
</template>
<style scoped>
  .todo-item {
    border-bottom: 1px solid #80808057;
  }

  .settings {
    opacity: 0;
    transition: all .3s ease-in-out;
  }

  .todo-item:hover {
    background: #31344d;
  }

  .todo-item:hover>.settings {
    opacity: 1;
  }

</style>
<script>
  export default {
    name: 'todo-item',
    props: ['index']
  }

</script>
