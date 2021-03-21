<template>
  <div id="app">
    <div class="flex-container">
      <menuBar @selectedTag="selected = $event"></menuBar>
      <drawContent :selected="selected"></drawContent>
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

.flex-container {
  display: flex;
  align-items: stretch;
  height: 100%;
}
</style>
