<template>
  <div id="app">
    <div class="container is-fullhd">
     <Navigation/>
     <Courses/>
     <Progress/>
    </div>
  </div>
</template>

<script>
import Navigation from '@/components/Navigation.vue'
import Courses from '@/components/Courses.vue'
import Progress from '@/components/Progress.vue'

export default {
  name: 'App',
  components: {
    Navigation,
    Courses,
    Progress
  }
}
</script>

<style lang="scss">
@import '@/assets/scss/index.scss';
  .container{
    display: flex;
    justify-content: space-between;
    // width: 100vw;
    // max-height: 100vh;
    background: $primary-color;
  }
</style>
