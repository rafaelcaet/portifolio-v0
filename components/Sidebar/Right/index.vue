<template>
    <div class="flex flex-col">
        <!-- Preview card: Find me -->
        <SidebarRightPreviewCard title="Find me">
            <SidebarRightPreviewCardItem v-for="findMe in findMeItems">
                <div>
                    <h2
                        class="font-bold font-jbmono text-gray-800 text-md dark:text-white"
                    >
                        {{ findMe.title }}
                    </h2>
                    <p class="text-sx font-jbmono text-gray-400">
                        {{ findMe.count }}
                    </p>
                </div>
            </SidebarRightPreviewCardItem>
        </SidebarRightPreviewCard>
    </div>
</template>
<script setup>
const findMeItems = ref([
    { icon: '', title: 'GitHub', count: 'rafaelcaet' },
    { icon: '', title: 'LinkedIn', count: 'Rafael Caetano' },
    { icon: '', title: 'Email', count: 'fael.caetsantos@gmail.com' },
    { icon: '', title: 'Instagram ', count: '@_rafaelcaetano' },
])
</script>
