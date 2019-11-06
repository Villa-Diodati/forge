<template>
  <main>
    <h1 v-if='!type'>Create</h1>
    <ul v-if='!type'>
      <li>New Item</li>
      <li>New Class</li>
      <li>New Spell</li>
    </ul>
  </main>
</template>

<script>
export default {
  name: 'Create',
  data: function () {
    return {
      type: '',
      content: {},
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='scss' scoped>
@import '../constants/scss-variables.scss';

h2 {
  margin: 0 0 40px;
}
main {
  width: 100%;
  height: calc(100% - 50px);
  display: flex;
  justify-content: center;
  align-items: center;
  box-sizing: border-box;
}

ul {
  margin: 40px;
  padding: 30px 0;
  border-left: 1px solid $forgeGrey;
}
li {
  text-align: left;
  margin: 40px 40px;
  font-size: 30px;
  cursor: pointer;

  &:hover {
    color: $forgeOrange;
  }
}

</style>
