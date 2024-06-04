<template>
    <div class="mt-16 ml-2 mr-2">
        <div class="items-center">
            <h1
                class="text-xl font-bold text-gray-800 dark:text-gray-100 ml-44 mb-4"
            >
                A bit about me...
            </h1>
            <div
                class="text-base space-y-4 space-x-1 text-gray-800 dark:text-gray-100"
            >
                <p>
                    &nbsp;&nbsp;&nbsp;&nbsp;I am Rafael Caetano, a backend
                    developer passionate about technology and learning.
                </p>
                <p>
                    &nbsp;&nbsp;&nbsp;&nbsp; I began my studies around 2012 and
                    completed a technical course in Industrial Automation in
                    2015 at Colégio Católica Padre de Man. In 2016, I started my
                    undergraduate degree in Computer Engineering at the Federal
                    University of Ouro Preto, where I gained substantial
                    knowledge in software development. In mid-2022, I had my
                    first opportunity to enter the job market when I was invited
                    to participate in building a startup called Cali Finance,
                    which developed a payment system using cryptocurrencies with
                    payments made per second. Due to the vast amount of
                    knowledge I was exposed to there, I decided to pause my
                    graduation (I was in the 9th/10th semester of the course)
                    and dedicate 100% of my time to learning even more about
                    software development. This experience lasted until February
                    2024 (02/24).
                </p>
                <p>
                    &nbsp;&nbsp;&nbsp;&nbsp;During my journey, I had the chance
                    to meet incredible people who motivated me to start some
                    "side projects", though unfortunately, none of them were
                    completed. These projects include a FiveM (GTAV) server and
                    a decentralized freelancing platform.
                </p>
                <p>
                    &nbsp;&nbsp;&nbsp;&nbsp;Currently, I'm focused on further
                    enhancing my skills as a developer by studying and learning
                    new languages and stacks.
                </p>
            </div>
            <div>
                <h1
                    class="mt-10 text-xl font-bold text-gray-800 dark:text-gray-100 ml-44 mb-6"
                >
                    Skills and levels
                </h1>
                <div
                    class="text-base items-center ml-16 grid grid-flow-col grid-rows-2 text-gray-800 dark:text-gray-100"
                >
                    <div>
                        <h2>team works</h2>
                        <UserGroupIcon class="size-20" />
                    </div>
                    <div>
                        <h2>English</h2>
                        <TranslateIcon class="size-20" />
                    </div>

                    <div>
                        <h2>Dedicated</h2>
                        <HeartIcon class="size-20" />
                    </div>
                    <div>
                        <h2>Portuguese</h2>
                        <TranslateIcon class="size-20" />
                    </div>
                    <div>
                        <h2>Communication</h2>
                        <ChatIcon class="size-20" />
                    </div>
                    <div>
                        <h2>Funny</h2>
                        <EmojiHappyIcon class="size-20" />
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
import {
    UserGroupIcon,
    HeartIcon,
    ChatIcon,
    TranslateIcon,
    EmojiHappyIcon,
} from '@heroicons/vue/outline'
</script>
