<template>
<div class="header row justify-center">
<h3 class="q-pa"> VIRROSHAN KUMAR </h3>
</div>
</template>

<script>
export default {
name : 'IntroBanner',
}
</script>

<style lang="scss" scoped>

.header {
  background : black;
}

h3 {
  text-align: center;
  animation: glow 1s ease-in-out infinite alternate;
  font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
  color: white;

}

@keyframes glow {
  from {
    text-shadow: 0 0 1px rgb(6, 6, 6), 0 0 2px rgb(45, 45, 45), 0 0 3px #5c5d5c, 0 0 4px #848684, 0 0 5px #c2c3c3, 0 0 6px #00ff4c, 0 0 70px #008cff;
  }


  to {
    text-shadow: 0 0 2px rgb(71, 55, 55), 0 0 3px #797878, 0 0 4px #969595, 0 0 5px #c1c0c0, 0 0 6px #ffffff, 0 0 7px #ff0202, 0 0 80px #f6ff00;
  }
}

</style>
