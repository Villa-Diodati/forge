<template>
  <main class="hello">
    <h1>Welcome to the Forge</h1>
    <h2>A D&D Creation Tool</h2>
    <p>
      The Forge creates items, classes, spells, and... stuff by building lists of effects that the thing has.  If this is your first time using the Forge, please check out some examples (pending).
    </p>
  </main>
</template>

<script>
export default {
  name: 'Home',
  props: {
    msg: String,
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h2 {
  margin: 0 0 40px;
}
main {
  text-align: center;
  margin: 15% 25%;
}

</style>
