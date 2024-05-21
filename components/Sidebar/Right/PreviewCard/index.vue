<template>
    <div
        class="m-2 border rounded-2xl bg-gray-50 dark:bg-dim-700 overflow-hidden"
        :class="thinBorderColor"
    >
        <h1
            class="p-3 text-xl font-extrabold text-gray-900 border-b dark:text-white"
            :class="thinBorderColor"
        >
            {{ props.title }}
        </h1>

        <slot> </slot>
    </div>
</template>
<script setup>
const { thinBorderColor, defaultTransition } = useTailwindConfig()

const props = defineProps({
    title: {
        type: String,
        required: true,
    },
})
</script>
