<script setup>
import SquareScales from '../components/SquareScales.vue'
import TheFooter from '@/components/TheFooter.vue'
</script>

<template>
  <main>
    <SquareScales v-for="n in 200" :key="n" class="square" />
    <TheFooter />
  </main>
</template>

<style scoped>
.square {
  padding: 48px;
}

main {
  position: relative;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  width: 100vw;
  height: 100vh;
  background-color: rgba(218, 215, 191, 0.802);
  gap: 40px;
  overflow-y: hidden;
  overflow-x: hidden;
  font-family: 'IBM Plex Mono';
  color: #333;

  border-radius: 6px;

  box-shadow:
    0 4px 12px rgba(0, 0, 0, 0.321),
    0 2px 4px rgba(0, 0, 0, 0.263);
}

main::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
</style>
