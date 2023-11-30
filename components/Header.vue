<script setup lang='ts'>
const datas = ['首页', '传媒故事', '传媒风采', '学院介绍', '联系我们']
const paths = ['/', '/story', '/media', '/introduce', '/contact']
</script>

<template>
  <div h-10 flex border-b bg-gray-1>
    <span
      v-for="(item, index) in datas" :key="index"
    ><NuxtLink :to="paths[index]">
      <span
        text="gray-8"

        inline-block h-10 w-70 rd-0 bg-gray-1 transition-2 btn hover-bg-gray-2
      >

        {{ item }}

      </span>
    </NuxtLink>
    </span>
  </div>
</template>
