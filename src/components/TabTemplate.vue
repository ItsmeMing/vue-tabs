<template>
    <div>
        <h1>{{ Header }}</h1>
        <p class="content">{{ Content }}</p>
    </div>
</template>

<script setup>
defineProps(["Header", "Content"]);
</script>

<style scoped lang="scss">
div {
    h1 {
        font-weight: 600;
        font-size: 30px;
        margin: 20px 0;
    }
}
</style>