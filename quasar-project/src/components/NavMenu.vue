<template>
  <div class="col q-pa-sm" align="left">
    <div class="float-child-left">
      <q-btn fixed round class="row" size="25px" color="black" icon="home">
        <q-tooltip
          transition-show="scale"
          transition-hide="scale"
          anchor="center right"
          self="center left"
          :offset="[20, 20]"
        >
          <strong>HOME</strong>
        </q-tooltip>
      </q-btn>
      <q-btn fixed round class="row" size="25px" color="black" icon="work">
        <q-tooltip
          transition-show="scale"
          transition-hide="scale"
          anchor="center right"
          self="center left"
          :offset="[20, 20]"
        >
          <strong>WORK</strong>
        </q-tooltip>
      </q-btn>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavMenu",
};
</script>

<style lang="scss" scopped>
.float-child-left {
  min-width: 1%;
  float: left;
  margin-top: 20%;
  color: rgb(70, 70, 70);
}
</style>
