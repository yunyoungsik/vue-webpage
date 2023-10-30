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
  <Header />
  <main>
    <Slider />
    <Image />
    <ImageText />
    <Card />
    <Banner />
    <Text />
  </main>
  <Footer />
</template>