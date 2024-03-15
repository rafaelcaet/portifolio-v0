<template>
    <div class="h-screen flex flex-col">
        <div
            class="p-2 my-2 rounded-full hover:bg-blue-50 w-min dark:hover:bg-white/20"
            :class="defaultTransition"
        >
            <nuxt-link to="/">
                <div class="w-8 h-8">
                    <LogoSocialMedia />
                </div>
            </nuxt-link>
        </div>
        <div class="mt-2 space-y-3">
            <!-- home icon -->
            <SidebarLeftTab active>
                <template v-slot:icon>
                    <HomeIcon />
                </template>
                <template v-slot:name> Home </template>
            </SidebarLeftTab>

            <!-- hashtag icon -->
            <SidebarLeftTab>
                <template v-slot:icon>
                    <HashtagIcon />
                </template>
                <template v-slot:name> Explore </template>
            </SidebarLeftTab>

            <!-- bell icon -->
            <SidebarLeftTab>
                <template v-slot:icon>
                    <BellIcon />
                </template>
                <template v-slot:name> Notifications </template>
            </SidebarLeftTab>

            <!-- inbox icon -->
            <SidebarLeftTab>
                <template v-slot:icon>
                    <InboxIcon />
                </template>
                <template v-slot:name> Messages </template>
            </SidebarLeftTab>

            <!-- bookmark icons -->
            <SidebarLeftTab>
                <template v-slot:icon>
                    <BookmarkIcon />
                </template>
                <template v-slot:name> Bookmarks </template>
            </SidebarLeftTab>

            <!-- documentText icon -->
            <SidebarLeftTab>
                <template v-slot:icon>
                    <DocumentTextIcon />
                </template>
                <template v-slot:name> Lists </template>
            </SidebarLeftTab>

            <!-- user icon -->
            <SidebarLeftTab>
                <template v-slot:icon>
                    <UserIcon />
                </template>
                <template v-slot:name> Profile </template>
            </SidebarLeftTab>

            <!-- dotsCircleHorizontal icon -->
            <SidebarLeftTab>
                <template v-slot:icon>
                    <DotsCircleHorizontalIcon />
                </template>
                <template v-slot:name> More </template>
            </SidebarLeftTab>
        </div>
    </div>
</template>
<script setup>
import { HomeIcon } from '@heroicons/vue/solid'
import {
    HashtagIcon,
    BellIcon,
    InboxIcon,
    BookmarkIcon,
    DocumentTextIcon,
    UserIcon,
    DotsCircleHorizontalIcon,
} from '@heroicons/vue/outline'
const { defaultTransition } = useTailwindConfig()
</script>
