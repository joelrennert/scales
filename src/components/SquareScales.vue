<template>
  <div class="square"><a href="#"></a></div>
</template>

<script></script>

<style scoped>
.square {
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 2rem;
  border-radius: 25%;
  box-shadow:
    8px 8px 18px rgba(0, 0, 0, 0.348),
    -8px -8px 18px rgba(218, 215, 191, 0.6);
  transform: rotate(100deg) skewX(10deg) skewY(10deg);
  animation: pulse 4s ease-in-out infinite;
}

@keyframes pulse {
  0% {
    transform: scale(1.3) rotate(100deg) skewX(10deg) skewY(10deg);
  }
  50% {
    transform: scale(1.38) rotate(100deg) skewX(10deg) skewY(10deg);
  }
  100% {
    transform: scale(1.3) rotate(100deg) skewX(10deg) skewY(10deg);
  }
}
</style>
