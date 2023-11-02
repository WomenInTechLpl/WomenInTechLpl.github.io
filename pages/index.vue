<template>
    <div class="background-image container"></div>
    <div class="overlay-div"></div>
    <div class="text-div text_shadows">
        Coming Soon...
    </div>
</template>

<style scoped>
.body {
    font-family: bungee, sans-serif;
}
.background-image {
    width: 100%;
    height: 100%;
    background-image: url('../assets/images/IMG_3941.jpg');
    background-size: cover;
}

.container {
    position: relative;
}

.overlay-div {
    width: 100%;
    height: 100vh;
    position: absolute;
    background-color: #000;
    top: 0;
    left: 0;
    opacity: 0.55;
}
.text-div {
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    text-align: center;
    vertical-align: middle;
    line-height: 100vh;
    color: #fff;
    font-weight: bold;
}


*,
*::before,
*::after {
  box-sizing: border-box;
}

body {
  min-height: 100vh;
  /* font-family: canada-type-gibson, sans-serif; */
  font-weight: 300;
  font-size: 1rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
  overflow: hidden;
}

.text_shadows {
  text-shadow: 3px 3px 0 #f49b90, 6px 6px 0 #f28b7d,
    9px 9px #f07a6a, 12px 12px 0 #ee6352;
  font-family: bungee, sans-serif;
  font-weight: 400;
  text-transform: uppercase;
  font-size: calc(2rem + 5vw);
  text-align: center;
  margin: 0;
  color: #f6aca2;
  /* color: transparent;
  background-color: white;
  background-clip: text; */
  animation: shadows 1.2s ease-in infinite, move 1.2s ease-in infinite;
  letter-spacing: 0.4rem;
}

@keyframes shadows {
  0% {
    text-shadow: none;
  }
  10% {
    text-shadow: 3px 3px 0 #f49b90;
  }
  20% {
    text-shadow: 3px 3px 0 #f49b90,
      6px 6px 0 #f28b7d;
  }
  30% {
    text-shadow: 3px 3px 0 #f49b90,
      6px 6px 0 #f28b7d, 9px 9px #f07a6a;
  }
  40% {
    text-shadow: 3px 3px 0 #f49b90,
      6px 6px 0 #f28b7d, 9px 9px #f07a6a,
      12px 12px 0 #ee6352;
  }
  50% {
    text-shadow: 3px 3px 0 #f49b90,
      6px 6px 0 #f28b7d, 9px 9px #f07a6a,
      12px 12px 0 #ee6352;
  }
  60% {
    text-shadow: 3px 3px 0 #f49b90,
      6px 6px 0 #f28b7d, 9px 9px #f07a6a,
      12px 12px 0 #ee6352;
  }
  70% {
    text-shadow: 3px 3px 0 #f49b90,
      6px 6px 0 #f28b7d, 9px 9px #f07a6a;
  }
  80% {
    text-shadow: 3px 3px 0 #f49b90,
      6px 6px 0 #f28b7d;
  }
  90% {
    text-shadow: 3px 3px 0 #f49b90;
  }
  100% {
    text-shadow: none;
  }
}

@keyframes move {
  0% {
    transform: translate(0px, 0px);
  }
  40% {
    transform: translate(-12px, -12px);
  }
  50% {
    transform: translate(-12px, -12px);
  }
  60% {
    transform: translate(-12px, -12px);
  }
  100% {
    transform: translate(0px, 0px);
  }
}
</style>