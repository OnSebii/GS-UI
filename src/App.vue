<template>
  <div id="app">
    <div class="row">
      <menuBar class="col-sm-1-half" @selectedTag="selected = $event"></menuBar>
      <drawContent class="col-11" :selected="selected"></drawContent>
    </div>
  </div>
</template>

<script>
import menuBar from './components/menuBar.vue';
import drawContent from '@/components/drawContent.vue';

export default {
  data() {
    return {
      selected: undefined,
    };
  },
  name: 'App',
  components: {
    menuBar,
    drawContent,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.col-sm-1-half {
  position: relative;
  min-height: 1px;
}

@media (min-width: 768px) {
  .col-sm-1-half {
    float: left;
    width: 29.16666667%;
  }
}

.row {
  margin: 0 !important;
}
</style>
