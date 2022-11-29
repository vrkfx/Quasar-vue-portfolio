
<template>
  <div >

      <q-card class="my-card">
        <img :src="projectImage" />

        <q-card-section>
          <div class="text-overline text-orange-8">{{ projectStack }}</div>
          <div class="text-h5 q-mt-sm q-mb-xs">{{ projectName }}</div>
          <div class="text-caption text-grey">
            {{ projectDesc }}
          </div>
        </q-card-section>

        <q-card-section class="q-pt-none">
          <div class="text-subtitle2">{{ projectLink }}</div>
        </q-card-section>
      </q-card>

  </div>

</template>

<script>
export default {

name : 'ProjectCard',

props: {
    projectName: {
      type: String,
      required: true,
    },

    projectStack: {
      type: String,
      required: true,
    },

    projectDesc: {
      type: String,
    },

    projectLink: {
      type: String,
      default: "",
    },

    projectImage: {
      type: String,
      default: "",
    },
  },

  data() {},

setup() {
  return {
    img: "https://cdn.shopify.com/s/files/1/0306/6419/6141/articles/coding_languages_900x.png?v=1619126283",
  };
},

}
</script>

<style lang="scss" scopped>

.my-card {
  width: 100%;
  float: right;
  color:rgb(68, 68, 68);
  background: black;
  // border-style: solid;
  border-radius: 15px;
}

</style>
