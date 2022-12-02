<template>
  <div class="sticky" >

      <q-btn fixed round class="row btn" size="15px" color="black" icon="home">
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
      <q-btn fixed round class="row btn" size="15px" color="black" icon="work">
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

</template>

<script>
export default {
  name: "NavMenu",
};
</script>

<style lang="scss" scopped>

div.sticky {
  background: rgb(47, 47, 47);

  float: left;
 // margin: auto;
 height: 1000px;
  color: rgb(70, 70, 70);
  position: -webkit-sticky;
  position: sticky;
  top: 0;
  background-color: rgb(35, 35, 35);
  margin: auto;
  padding:5px;

padding-top: 25%;
}
.btn{
  padding:10px;
}
</style>
