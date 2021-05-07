<template>
    <div class="absolute top-0 left-0 w-full h-full">
        <div class="max-w-xl mx-auto mt-16">
            <div class="flex justify-between">
                <h1 class="text-white todo text-4xl font-bold">TODO</h1>
                <span class="text-white">ICON</span>
            </div>
            <div class="search rounded-lg p-5 mt-4 flex items-center">
                <i class="fa fa-plus text-white mr-5"></i>
                <input type="text" placeholder="Crear nueva tarea hoy">
            </div>
            <div class="content-list rounded-lg mt-6">
                <slot></slot>
                <footer class="p-5 flex justify-between items-center">
                    <small class="text-gray-600 font-bold cursor-pointer">4 TAREAS</small>
                    <div class="flex">
                        <div class="cursor-pointer mr-2 text-blue-600">...</div>
                        <div class="cursor-pointer mr-2 text-blue-600">...</div>
                        <div class="cursor-pointer mr-2 text-blue-600">..</div>
                    </div>
                    <small class="text-gray-600 font-bold clear-completed cursor-pointer">
                        LIMPIAR
                    </small>
                </footer>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'todo-app-list'
}
</script>
<style scoped>
    .search {
        background: var(--color-secondary);
    }
    .search input {
        border: none;
        background: #0000;
        box-sizing: border-box;
        width: 100%;
        outline: none;
        color: var(--text-primary);
    }
    .todo {
        letter-spacing: 4px;
    }
    .content-list {
        background: var(--color-secondary);
    }
</style>