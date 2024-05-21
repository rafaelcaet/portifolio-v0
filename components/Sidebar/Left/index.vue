<template>
    <div class="h-screen flex flex-col">
        <div
            class="p-2 my-2 rounded-full hover:bg-blue-50 w-min dark:hover:bg-white/20"
            :class="defaultTransition"
        >
            <nuxt-link to="/">
                <div
                    class="w-14 h-11 text-sm font-jbmono text-gray-800 dark:text-gray-100"
                >
                    RAFAEL CAETANO
                </div>
            </nuxt-link>
        </div>
        <div class="mt-2 space-y-3">
            <!-- Home icon -->
            <SidebarLeftTab active path="/home">
                <template v-slot:icon>
                    <HomeIcon />
                </template>
                <template v-slot:name> Home </template>
            </SidebarLeftTab>

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
            <SidebarLeftTab>
                <template v-slot:icon>
                    <InboxIcon />
                </template>
                <template v-slot:name> Contacts </template>
            </SidebarLeftTab>
        </div>
    </div>
</template>
<script setup>
import { HomeIcon } from '@heroicons/vue/solid'
import { HashtagIcon, InboxIcon, UserIcon } from '@heroicons/vue/outline'
const { defaultTransition } = useTailwindConfig()
</script>
