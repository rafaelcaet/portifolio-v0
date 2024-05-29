<template>
    <div class="h-screen flex flex-col">
        <div
            class="p-2 my-2 rounded-full hover:bg-blue-50 w-min dark:hover:bg-white/20"
            :class="defaultTransition"
        >
            <nuxt-link to="/">
                <div
                    class="w-14 h-11 m-2 text-bold text-sm font-jbmono text-gray-800 dark:text-gray-100"
                >
                    Rafael Caetano
                </div>
            </nuxt-link>
        </div>
        <div class="mt-2 space-y-3">
            <!-- User icon -->
            <SidebarLeftTab active path="/about">
                <template v-slot:icon>
                    <UserIcon />
                </template>
                <template v-slot:name> About </template>
            </SidebarLeftTab>

            <!-- hashtag icon -->
            <SidebarLeftTab active path="/projects">
                <template v-slot:icon>
                    <HashtagIcon />
                </template>
                <template v-slot:name> Projects </template>
            </SidebarLeftTab>

            <!-- inbox icon -->
            <SidebarLeftTab active path="/contact">
                <template v-slot:icon>
                    <InboxIcon />
                </template>
                <template v-slot:name> Contact </template>
            </SidebarLeftTab>
        </div>
    </div>
</template>
<script setup>
import { HashtagIcon, InboxIcon, UserIcon } from '@heroicons/vue/outline'
const { defaultTransition } = useTailwindConfig()
</script>
