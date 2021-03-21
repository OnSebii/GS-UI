<template>
  <div>
    <div class="container">
      <div class="settingsBox">
        <fieldset class="drawBox leftBox">
          <legend>Aimbot</legend>
          <a
            >Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos
            et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur
            sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea
            rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.</a
          >
        </fieldset>
        <fieldset class="drawBox rightBox">
          <legend>Other</legend>
          <a
            >Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos
            et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur
            sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea
            rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.</a
          >
        </fieldset>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    selected: Number,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container {
  background-image: url('../img/gsChains.png');
  padding: 25px;
  border-left: 1px solid #3c3c3c;
  height: 100%;
}

.settingsBox {
  display: flex;
  align-items: stretch;
  height: 100%;
}

.leftBox {
  margin-right: 12px;
}
.rightBox {
  margin-left: 12px;
}

.drawBox {
  box-sizing: border-box;
  border: 1px solid #3c3c3c;
  background-color: #171717;
}

legend {
  color: #c8c8c8;
  font-size: 15px;
  font-weight: bold;
}
</style>
