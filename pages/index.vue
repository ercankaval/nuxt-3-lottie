<script setup>
import { Vue3Lottie } from 'vue3-lottie'
import CarAnimation from '~/assets/lottie/car-animation.json'
import HeartAnimation from '~/assets/lottie/heart.json'
import LoadingAnimation from '~/assets/lottie/loading.json'

</script>

<template>
  <div style="display: flex; flex-direction: column; padding: 150px; align-items: center">
  <client-only>
    <h1>Animation Link</h1>
    <Vue3Lottie
        animationLink="https://assets10.lottiefiles.com/packages/lf20_soCRuE.json"
        :height="200"
        :width="200"
    />

    <h1>Animation Data: Car</h1>
    <Vue3Lottie
        :animationData="CarAnimation"
        :height="200"
        :width="200"
        :play-on-hover="true"
    />

    <h1>Animation Data: Heart</h1>
    <Vue3Lottie
        :animationData="HeartAnimation"
        :height="200"
        :width="200"
    />

    <h1>Animation Data: Loading</h1>
    <Vue3Lottie
        :animationData="LoadingAnimation"
        :height="200"
        :width="200"
        :pause-on-hover="true"
    />
  </client-only>
  </div>
</template>


<style lang="scss" scoped>

</style>