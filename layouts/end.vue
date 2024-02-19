<template>
    <div class="relative h-full" style="background: linear-gradient(rgba(255, 255, 255, 0.7), rgba(255, 255, 255, 0.7)), url('/bg.jpeg');">
        <div class="relative h-full" style="background: linear-gradient(#ffffff33, rgba(255, 255, 255, 0.2)), url('/circle.png') ;background-size: cover;">
            <div class="bg-[#323681] w-full h-12">
                <div class="flex justify-between items-center h-full px-5">
                    <img src="/LeftLogo.png" class="h-9" />
                    <img src="/RightLogo.png" class="h-9" />
                </div>
            </div>
            <!-- 正文区 -->
            <div class ="slidev-layout end w-full relative pt-45 px-15">
                <div class="my-auto">
                    <slot />
                </div>
            </div>

            <!-- 右下角页码 -->
            <div class="z-10 absolute bottom-3 right-8 text-xs text-gray-500">
                {{ $slidev.nav.currentPage }} / {{ $slidev.nav.total}}
            </div>
        </div>
    </div>
</template>
