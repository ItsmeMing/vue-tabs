<script setup>
import {inject} from "vue";
defineProps(["title", "selectedTitle"]);
const selectedTitle = inject("selectedTitle");
</script>

<template>
    <div class="tab__content" v-if="title === selectedTitle">
        <slot />
    </div>
</template>

<style scoped lang="scss">
.tab__content {
    overflow: auto;
}
</style>
