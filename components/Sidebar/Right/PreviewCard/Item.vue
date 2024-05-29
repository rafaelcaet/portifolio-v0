<template>
    <div
        class="p-3 hover:bg-gray-100 cursor-pointer dark:hover:bg-dim-300 border-b"
        :class="wrapperClasses"
    >
        <slot></slot>
    </div>
</template>
<script setup lang="ts">
const wrapperClasses = computed(() => `${defaultTransition} ${thinBorderColor}`)
const { defaultTransition, thinBorderColor } = useTailwindConfig()
const props = defineProps({
    active: {
        type: Boolean,
        default: false,
    },
    path: String,
})
</script>
