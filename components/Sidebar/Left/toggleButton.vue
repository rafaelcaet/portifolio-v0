<template>
    <div class="flex text-black dark:text-white dark:border-white bg-red-400">
        <button @click="toggleState">Button text</button>
    </div>
</template>
<script setup lang="ts">
const isCollapsed = ref(false)

const toggleState = () => {
    isCollapsed.value = !isCollapsed.value
}
</script>
