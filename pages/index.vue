<template>
    <div class="font-jbmono">
        <MainSection title="Home" :loading="loading">
            <MainContentHome />
        </MainSection>
    </div>
</template>
<script setup>
const loading = ref(false)
</script>
