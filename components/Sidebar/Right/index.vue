<template>
    <div class="flex flex-col">
        <!-- Preview card: Find me -->
        <SidebarRightPreviewCard title="Find me">
            <SidebarRightPreviewCardItem v-for="findMe in findMeItems">
                <div>
                    <h2 class="font-bold text-gray-800 text-md dark:text-white">
                        {{ findMe.title }}
                    </h2>
                    <p class="text-sx text-gray-400">
                        {{ findMe.count }}
                    </p>
                </div>
            </SidebarRightPreviewCardItem>
        </SidebarRightPreviewCard>
    </div>
</template>
<script setup>
const findMeItems = ref([
    { icon: '', title: 'Instagram ', count: '@_rafaelcaetano' },
    { icon: '', title: 'GitHub', count: 'rafealcaet' },
    { icon: '', title: 'LinkedIn', count: 'Rafael Caetano' },
])
</script>
