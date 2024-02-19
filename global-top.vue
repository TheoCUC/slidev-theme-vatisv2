<!-- global-top.vue -->
<template>
    <footer v-if="$slidev.nav.currentLayout == 'default'" class="absolute top-0 right-20 p-2.5 text-lg text-gray-400 flex space-x-5">
        <div v-for="(item,index) in $slidev.configs.sections">
            <p v-if="($slidev.nav.currentPage >= item[1]) && ((!$slidev.configs.sections[index+1]) || ($slidev.nav.currentPage < $slidev.configs.sections[index+1][1]))" class="font-[KaiTi] text-white" @click="$slidev.nav.go(item[1])">{{ item[0] }}</p>
            <p v-else class="font-[KaiTi]" @click="$slidev.nav.go(item[1])">{{ item[0] }}</p>
        </div>
    </footer>


    <footer v-if="$slidev.nav.currentLayout == 'end'" class="absolute top-0 right-20 p-2.5 text-lg text-gray-400 flex space-x-5">
        <div v-for="(item,index) in $slidev.configs.sections">
            <p class="font-[KaiTi] text-white" @click="$slidev.nav.go(item[1])">{{ item[0] }}</p>
        </div>
    </footer>
</template>