<template>
  <div>
    <div class="ui">
      <a class="gsIcons" @click="selectedTag(1)" :class="{ gsIconsSelected: selected == 1 }">A</a>
      <br />
      <a class="gsIcons" @click="selectedTag(2)" :class="{ gsIconsSelected: selected == 2 }">G</a>
      <br />
      <a class="gsIcons" @click="selectedTag(3)" :class="{ gsIconsSelected: selected == 3 }">C</a>
      <br />
      <a class="gsIcons" @click="selectedTag(4)" :class="{ gsIconsSelected: selected == 4 }">D</a>
      <br />
      <a class="gsIcons" @click="selectedTag(5)" :class="{ gsIconsSelected: selected == 5 }">E</a>
      <br />
      <a class="gsIcons" @click="selectedTag(6)" :class="{ gsIconsSelected: selected == 6 }">F</a>
      <br />
      <img alt="Config" src="../img/cfg.svg" @click="selectedTag(7)" :class="{ gsIconsSelected: selected == 7 }" />
      <br />
      <p @click="selectedTag(8)" :class="{ gsIconsSelected: selected == 8 }">Lua</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      selected: undefined,
    };
  },
  methods: {
    selectedTag(num) {
      this.selected = num;
      return this.$emit('selectedTag', num);
    },
  },
  created() {
    this.selectedTag(1);
  },
};
</script>

<!-- Add "scoped" attribute to amit CSS to this component only -->
<style scoped>
.gsIcons {
  font-family: 'menu_font';
  font-size: 65px;
  width: 80px;
  display: inline-block;
  text-align: center;
  color: #5a5a5a;
  background-color: #0c0c0c;
}

.gsIconsSelected {
  color: #d2d2d2;
  background-image: url('../img/gsChains.png');
  background-repeat: repeat;
  border-top: 1px solid #3c3c3c;
  border-bottom: 1px solid #3c3c3c;
}

.ui {
  margin-top: 10px;
}

img {
  width: 80px;
  background-color: #0c0c0c;
}

p {
  width: 80px;
  font-size: 25px;
  margin: 10px 0px;
  text-align: center;
  background-color: #0c0c0c;
  color: #5a5a5a;
  font-weight: bold;
}

@font-face {
  font-family: 'menu_font';
  src: url('../fonts/menu_font.ttf') format('truetype');
}
</style>
