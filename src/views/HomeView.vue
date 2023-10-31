<script setup>
import Header from "@/components/Header.vue"
import Footer from "@/components/Footer.vue"
import Slider from "@/components/Slider.vue"
import Image from "@/components/Image.vue"
import ImageText from "@/components/ImageText.vue"
import Card from "@/components/Card.vue"
import Banner from "@/components/Banner.vue"
import Text from "@/components/Text.vue"
</script>

<template>
  <Header element="nexon" />
  <main>
    <Slider element='nexon' title='슬라이드 유형01' />
    <Image element='nexon section' title='포트폴리오가 실력이다.' />
    <ImageText element='nexon section' title='이미지 텍스트 유형' />
    <Card element='nexon section' title='웹스토리보이 강의' />
    <Banner element='nexon section' title='배너 영역' />
    <Text element='nexon section' title='텍스트 유형01' />
  </main>
  <Footer element='nexon section' title='푸터 영역' />
</template>