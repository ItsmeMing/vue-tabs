<script setup>
import TabWrapper from "./components/TabWrapper.vue";
import VueTab from "./components/VueTab.vue";
import TabTemplate from "./components/TabTemplate.vue";
</script>

<template>
    <div id="app">
        <TabWrapper>
            <VueTab title="Mails"
                ><TabTemplate
                    Header="Mails"
                    Content="Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis praesentium cumque magnam odio iure quidem, quod illum numquam possimus obcaecati commodi minima assumenda consectetur culpa fuga nulla ullam. In, libero.
                    Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis praesentium cumque magnam odio iure quidem, quod illum numquam possimus obcaecati commodi minima assumenda consectetur culpa fuga nulla ullam. In, libero."
            /></VueTab>
            <VueTab title="Alarms"
                ><TabTemplate
                    Header="Alarms"
                    Content="Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis praesentium cumque magnam odio iure quidem, quod illum numquam possimus obcaecati commodi minima assumenda consectetur culpa fuga nulla ullam. In, libero.
                    Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis praesentium cumque magnam odio iure quidem, quod illum numquam possimus obcaecati commodi minima assumenda consectetur culpa fuga nulla ullam. In, libero."
            /></VueTab>
            <VueTab title="Movies"
                ><TabTemplate
                    Header="Movies"
                    Content="Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis praesentium cumque magnam odio iure quidem, quod illum numquam possimus obcaecati commodi minima assumenda consectetur culpa fuga nulla ullam. In, libero.
                    Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis praesentium cumque magnam odio iure quidem, quod illum numquam possimus obcaecati commodi minima assumenda consectetur culpa fuga nulla ullam. In, libero.
                    Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis praesentium cumque magnam odio iure quidem, quod illum numquam possimus obcaecati commodi minima assumenda consectetur culpa fuga nulla ullam. In, libero."
            /></VueTab>
        </TabWrapper>
    </div>
</template>

<style lang="scss" scoped>
#app {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 800px;
    height: 100vh;
    margin: 0 auto;
}
</style>
