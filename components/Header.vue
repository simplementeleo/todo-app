<template>
    <div>
        <header class="w-full relative h-64">
            <div class="absolute w-full h-full top-0 left-0 bg-gradient"></div>
        </header>
    </div>
</template>
<script>
export default {
    name: 'header-image'
}
</script>
<style scoped>
    .bg-gradient {
        background: linear-gradient(45deg, #b02781a8, #4915a7b0);
    }
    header {
        background: url('../assets/cloud-servers.jpg') no-repeat;
        background-size: cover;
        background-position: left;
        box-shadow: 0 10px 15px #2f15408c;
    }
</style>