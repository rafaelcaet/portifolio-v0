<template>
    <div class="font-jbmono">
        <MainSection title="About" :loading="loading">
            <MainContentAbout />
        </MainSection>
    </div>
</template>
<script setup>
const loading = ref(false)
</script>
