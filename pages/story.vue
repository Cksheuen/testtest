<script setup lang='ts'>
interface Data {
  name: string
  major: string
  introduction: string
  url: string
}
const datas: Data[] = [
  {
    name: '张朝夕',
    major: '1987级电编专业',
    introduction: '本人1987年就读于中国传媒大学广播电视编导专业，1991年毕业，获文学学士学位。继续前往华中科技大学攻读研究生并在20...',
    url: 'https://tvs.cuc.edu.cn/_upload/article/images/d1/b4/af739ad74184a3bfc346637c58d2/2e184639-a6fe-4dab-9aba-be4499f5c38a.jpg',
  },
  {
    name: '鹿郡',
    major: '1987级电导专业',
    introduction: '本人于九十年代初毕业于中国传媒大学电视学院电视剧导演专业。毕业后分配至甘肃电视台工作八年，历经各类电视节目制作...',
    url: 'https://tvs.cuc.edu.cn/_upload/article/images/4b/08/6148ddee4745851a977e0cac79c7/e40482bf-7b25-4810-b226-a16e6195ee9a.jpg',
  },
  {
    name: '郭志成',
    major: '1987级电摄专业',
    introduction: '本人毕业于中国传媒大学电视新闻专业，1991 年 7 月至 1996 年 3 月任天津电视台新闻部记者；1996 年 4 月至 2010 年 ...',
    url: 'https://tvs.cuc.edu.cn/_upload/article/images/2b/df/b145b7914b9a993417da09d3e2be/ed05d1f2-6ee3-45f8-9fc2-378ff1639071.jpg',
  },
  {
    name: '杨文军',
    major: '1988级电编专业',
    introduction: '1992年毕业于中国传媒大学电视系，现任中国电视剧导演协会常务理事，霍尔果斯非凡响影视制作有限公司创始人、董事长...',
    url: 'https://tvs.cuc.edu.cn/_upload/article/images/b1/e7/77666f5b4f6bba78c69c8f4292c4/f0c363f2-3590-4c52-9968-0b81bba368db.jpg',
  },
]
</script>

<template>
  <div text="left">
    <h1>中国传媒大学</h1>
    <div flex>
      <p inline-block>
        座谈会上，廖祥忠表示，在全党全国深入学习贯彻习近平总书记关于宣传思想文化工作的重要指示精神之际，曹局长一行莅临学校调研指导，学校师生深受鼓舞、 倍感振奋。他从创业奠基、跨越发展、升级腾飞、高质量发展四个时期梳理了中国传媒大学近70年的办学历程，深情回忆了中国传媒大学和国家广电总局深厚的历史渊源和血脉情感，回顾了中央广播事业局创建学校前身北京广播学院的光荣岁月， 并对广电总局长期以来对学校成长发展给予的殷切关怀、倾力付出和大力支持表示衷心感谢。
      </p>
      <img src="/cuc.jpg" inline-block h-50>
    </div>
    <h1>知名校友</h1>
    <div flex>
      <div v-for="(item, index) in datas" :key="index" mx-10 inline-block h-50 w-60>
        <img :src="item.url" alt="item.name">
        <p>{{ item.name }}</p>
        <p>{{ item.major }}</p>
        <p>{{ item.introduction }}</p>
      </div>
    </div>
  </div>
</template>
