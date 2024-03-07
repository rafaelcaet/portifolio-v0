<template>
  <div :class="{ dark: darkMode }">
    <div class="bg-white dark:bg-dim-900">
      <div class="min-h-full">
        <div
          class="grid grid-cols-12 mx-auto sm:px-6 lg:max-w-7xl lg:px-8 lg:gap-5"
        >
          <!-- Left sidebad -->
          <div
            class="border-2 border-red-500 md:block xs-col-span-1 xl:col-span-2"
          >
            <div class="sticky top-0">
              <SidebarLeft />
            </div>
          </div>
          <!-- Main content -->
          <div class="bg-dim-500"></div>
          <!-- Right sidebar -->
          <div class="bg-dim-200"></div>
          <div></div>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
const darkMode = ref(true);
</script>
