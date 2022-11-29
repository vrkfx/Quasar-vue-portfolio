<template>
  <q-layout view="lHh Lpr lFf">
    <q-page-container>
      <IntroBanner/>
</q-page-container>

    <q-drawer
      v-model="leftDrawerOpen"
      show-if-above
      bordered
    >
      <q-list>
        <q-item-label
          header
        >
          Essential Links
        </q-item-label>

        <EssentialLink
          v-for="link in essentialLinks"
          :key="link.title"
          v-bind="link"
        />
      </q-list>
    </q-drawer>


    <q-page-container>
      <!-- <div v-for="i in linksList" :key="i"> -->
        <!-- <div class="q-pa-md"> -->

          <div class="row">

          <ProjectCard
          class="col-12 col-md-4"
            v-for="i in projectList"
            :key="i"
            :projectName="i.projectName"
            :projectStack="i.projectStack"
            :projectDesc="i.projectDesc"
            :projectLink="i.projectLink"
            :projectImage="i.projectImage"
          />
        <!-- </div> -->

</div>

    </q-page-container>


    <!-- <q-page-container>
      <router-view />
    </q-page-container> -->
  </q-layout>
</template>

<script>
import { defineComponent, ref } from 'vue'
import EssentialLink from 'components/EssentialLink.vue'
import ProjectCard from 'src/components/ProjectCard.vue'
import IntroBanner from 'src/components/IntroBanner.vue'

const linksList = [
  {
    title: 'Introduction',
    caption: 'quasar.dev',
    icon: 'school',
    link: 'https://quasar.dev'
  },
  {
    title: 'Skills',
    caption: 'github.com/quasarframework',
    icon: 'watch',
    link: 'https://github.com/quasarframework'
  },
  {
    title: 'Projects',
    caption: 'chat.quasar.dev',
    icon: 'work',
    link: 'https://chat.quasar.dev'
  },
  {
    title: 'Contact',
    caption: 'forum.quasar.dev',
    icon: 'chat',
    link: 'https://forum.quasar.dev'
  },

]

const projectList = [
  {
    projectName: "Project Test One",
    projectStack: "VUE, DOCKER, QUASAR",
    projectDesc:
      "This project is my personal portfolio to show case my skills .",
    projectLink: "www.github.com/virroshan",
    projectImage:
      "https://cdn.shopify.com/s/files/1/0306/6419/6141/articles/coding_languages_900x.png?v=1619126283",
  },
  {
    projectName: "Project Test Two",
    projectStack: "VUE, DOCKER, QUASAR",
    projectDesc:
      "This project is my personal portfolio to show case my skills .",
    projectLink: "www.github.com/virroshan",
    projectImage:
      "https://cdn.shopify.com/s/files/1/0306/6419/6141/articles/coding_languages_900x.png?v=1619126283",
  },
  {
    projectName: "Project Test Three",
    projectStack: "VUE, DOCKER, QUASAR",
    projectDesc:
      "This project is my personal portfolio to show case my skills .",
    projectLink: "www.github.com/virroshan",
    projectImage:
      "https://cdn.shopify.com/s/files/1/0306/6419/6141/articles/coding_languages_900x.png?v=1619126283",
  },
  {
    projectName: "Project Test Four",
    projectStack: "VUE, DOCKER, QUASAR",
    projectDesc:
      "This project is my personal portfolio to show case my skills .",
    projectLink: "www.github.com/virroshan",
    projectImage:
      "https://cdn.shopify.com/s/files/1/0306/6419/6141/articles/coding_languages_900x.png?v=1619126283",
  },

];

export default defineComponent({
  name: 'MainLayout',

  components: {
    EssentialLink,
    ProjectCard,
    IntroBanner,
  },

  setup () {
    const leftDrawerOpen = ref(false)

    return {
      projectList,
      essentialLinks: linksList,
      leftDrawerOpen,
      toggleLeftDrawer () {
        leftDrawerOpen.value = !leftDrawerOpen.value
      }
    }
  }
})
</script>

<style lang="sass" scoped>

.row > div
  padding: 10px 15px
.row + .row
  margin-top: 1rem
</style>
