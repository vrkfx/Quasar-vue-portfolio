<template>
  <div class="main row">
    <h3 class="col q-pa title">VIRROSHAN KUMAR</h3>
    <div class=" col intro">
    <h4> ++ Introduction ++ </h4>
    </div>>
  </div>
</template>

<script>
export default {
  name: "IntroBanner",
};
</script>

<style lang="scss" scoped>

h3 {
  text-align: center;
  animation: glow 1s ease-in-out infinite alternate;
  font-family:Kanit Medium;
  color: white;
  margin: auto;

}

.main{
  display: flex;
  justify-content: center;
  align-items: center;
  height: 250px;
  border: 1px solid rgb(57, 58, 57);
}

.intro{
  color:white;

}

// @keyframes glow {
//   from {
//     text-shadow: 0 0 1px rgb(6, 6, 6), 0 0 2px rgb(39, 38, 38),
//       0 0 3px #3b3b3b, 0 0 3px #525252, 0 0 3px #6f7070, 0 0 3px #929191,
//       0 0 3px #c3c2c2;
//   }

//   to {
//     text-shadow: 0 0 2px rgb(195, 194, 194), 0 0 3px #797878, 0 0 4px #969595,
//       0 0 5px #c1c0c0, 0 0 3px #ffffff, 0 0 3px #ffd102, 0 0 3px #ff9100;
//   }
//}
</style>
