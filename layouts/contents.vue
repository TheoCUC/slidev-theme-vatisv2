<template>
    <div class="relative h-full" style="background: linear-gradient(rgba(255, 255, 255, 0.7), rgba(255, 255, 255, 0.7)), url('/bg.jpeg');">
        <img src="/VATIS.png" class="absolute right-3 top-3 h-18" />
      <div class="relative h-full z-1" style="background: linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0)), url('/contentsbg.png') ;background-size: cover;">
        <div class="absolute top-63 left-56 text-white flex flex-col items-center">
            <p class="text-4xl text-bold">目录</p>
            <p>CONTENTS</p>
        </div>

        <!-- 目录内容 -->
        <div class="h-full flex flex-col content-center justify-center ml-120 space-y-12">
            <div v-for="(item, index) in $slidev.configs.sections" class="  flex space-x-3 items-center ">
                <p class="text-5xl text-[#323681]">
                    {{ (index+1).toString().padStart(2, '0') }}
                </p>
                <img src="/gap.png" class="h-12"/>
                <p class="text-2xl text-bold font-700">
                    {{ item[0] }}
                </p>
            </div>
        </div>
        
      </div>
    </div>
  </template>
  