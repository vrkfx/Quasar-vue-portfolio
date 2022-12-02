<template>
  <div class="header row justify-center">
    <h3 class="q-pa">VIRROSHAN KUMAR</h3>
  </div>
</template>

<script>
export default {
  name: "IntroBanner",
};
</script>

<style lang="scss" scoped>
.header {
  background: black;
}

h3 {
  text-align: center;
  animation: glow 1s ease-in-out infinite alternate;
  font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
    "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
  color: white;
}

@keyframes glow {
  from {
    text-shadow: 0 0 1px rgb(6, 6, 6), 0 0 2px rgb(255, 255, 255),
      0 0 3px #e1e3e1, 0 0 4px #f2f2f2, 0 0 5px #d5d9d9, 0 0 6px #a19f9f,
      0 0 7px #b4b4b4;
  }

  to {
    text-shadow: 0 0 2px rgb(71, 55, 55), 0 0 3px #797878, 0 0 4px #969595,
      0 0 5px #c1c0c0, 0 0 6px #ffffff, 0 0 7px #ffd102, 0 0 8px #ff9100;
  }
}
</style>
