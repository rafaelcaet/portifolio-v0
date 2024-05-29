<template>
    <div class="flex flex-col">
        <!-- Preview card: Find me -->
        <SidebarRightPreviewCard title="Find me">
            <SidebarRightPreviewCardItem
                v-for="findMe in findMeItems"
                active
                path="/about"
            >
                <div>
                    <h2
                        class="font-bold font-jbmono text-gray-800 text-md dark:text-white"
                    >
                        {{ findMe.title }}
                    </h2>
                    <p class="text-sx font-jbmono text-gray-400">
                        {{ findMe.username }}
                    </p>
                </div>
            </SidebarRightPreviewCardItem>
        </SidebarRightPreviewCard>
    </div>
</template>
<script setup lang="ts">
const findMeItems = ref([
    {
        icon: '',
        title: 'GitHub',
        username: 'rafaelcaet',
        url: 'https://github.com/rafaelcaet',
    },
    {
        icon: '',
        title: 'LinkedIn',
        username: 'Rafael Caetano',
        url: 'https://www.linkedin.com/in/rafael-caetano-bb1a75266/',
    },
    {
        icon: '',
        title: 'Instagram',
        username: '@_rafaelcaetano',
        url: 'https://instagram.com/_rafaelcaetano',
    },
])
</script>
