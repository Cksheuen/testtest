<template>
  <main class="px-10 py-10 text-center">
    <audio src="/MO_YU - 卡农（钢琴+小提琴）.mp3" autoplay loop />
    <Header mb-10 />
    <slot />
    <Footer />
    <div class="mx-auto mt-5 text-center text-sm opacity-25">
      [Default Layout]
    </div>
  </main>
</template>
