<template>
  <div class='wrapper'>
    <div class='spinner-outer'>
    </div>
    <div class='spinner-inner'>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ForgeSpinner',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='scss' scoped>
@import '../constants/scss-variables.scss';

.wrapper {
  position: relative;
  margin: 0 auto;
  width: 100px;
  height: 100px;
}

.spinner-outer {
  margin: 0 auto;
  border: 30px solid black;
  background: $forgeOrange;
  box-sizing: border-box;
  width: 100px;
  height: 100px;
  overflow: hidden;
  border-radius: 25px;
  animation-name: spin;
  animation-duration: 7s;
  animation-iteration-count: infinite;
}

.spinner-inner {
  border-radius: 100%;
  position: absolute;
  width: 50px;
  height: 25px;
  background: black;
  right: 25px;
  bottom: 20px;
}

@-webkit-keyframes spin {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(270deg);
  }
}

/* Standard syntax */
@keyframes spin {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(270deg);
  }
}

</style>
