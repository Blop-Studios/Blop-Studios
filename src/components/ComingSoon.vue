<template>
  <div>
    <div class="coming-soon-container">
      <div class="coming-soon">Something Huge is Coming Soon!</div>
    </div>
  </div>
</template>

<style>
body {
  margin: 0;
  display: flex;
  font-family: "Satoshi", sans-serif;
  background-color: #000;
}

.coming-soon-container {
  font-size: 1.5rem;
  color: #fff;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  height: 100vh;
}

.coming-soon {
  font-size: 9vw;
  margin: 0;
  padding: 0;
  font-weight: 900;
  --bg-size: 400%;
  --color-one: hsl(15 90% 55%);
  --color-two: hsl(40 95% 55%);
  background: linear-gradient(90deg, var(--color-one), var(--color-two), var(--color-one))
    0 0 / var(--bg-size) 100%;
  color: transparent;
  -webkit-background-clip: text;
  background-clip: text;
  animation: animate-background 8s infinite linear;
}

@keyframes animate-background {
  to {
    background-position: var(--bg-size) 0;
  }
}
</style>
