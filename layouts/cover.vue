<template>
  <div class="relative h-full" style="background: linear-gradient(rgba(255, 255, 255, 0.7), rgba(255, 255, 255, 0.7)), url('/bg.jpeg');">

    <div class="relative h-full z-1" style="background: linear-gradient(rgba(255, 255, 255, 0.2), rgba(255, 255, 255, 0.2)), url('/circle.png') ;background-size: cover;">
      <img src="/CoverLeft.png" class="h-full absolute left-15 -z-10" />
      <img src="/VATIS.png" class="absolute right-3 top-3 h-18" />
      <div class="slidev-layout cover ml-80 mr-20">
        <div class="my-auto w-full">
          <slot />
        </div>
      </div>
    </div>
  </div>
</template>
