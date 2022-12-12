<script setup>
import {ref, useSlots, provide} from "vue";
const slots = useSlots();
const tabTitles = ref(slots.default().map((tab) => tab.props.title));
const selectedTitle = ref(tabTitles.value[0]);
provide("selectedTitle", selectedTitle);

const checkClickedTab = (tab) => {
    if (selectedTitle.value === tab) {
        return "active";
    } else return "";
};
</script>
    
<template>
    <div class="tabs">
        <ul class="tabs__nav">
            <li
                v-for="(tab, key) in tabTitles"
                :key="key"
                @click="selectedTitle = tab"
                :class="checkClickedTab(tab)"
            >
                {{ tab }}
            </li>
        </ul>
        <slot />
    </div>
</template>

<style scoped lang="scss">
.tabs {
    display: flex;
    height: 250px;
    padding: 20px 10px;
    border: 2px solid #009688;
    .tabs__nav {
        flex: 0 0 20%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        margin-right: 20px;
        li {
            flex-basis: 33.33%;
            display: flex;
            justify-content: center;
            align-items: center;
            width: 100%;
            padding: 10px 20px;
            cursor: pointer;
            border: 2px solid transparent;
            &:hover {
                background-color: rgba(0,150,136, 0.1);
            }
        }
        li.active {
            border-right-color: #009688;
        }
    }
}
</style>
