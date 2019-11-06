<template>
  <nav>
    <ul>
      <li>Create</li>
      <li>Edit</li>
      <li>Help</li>
    </ul>
    <h2>The Forge</h2>
  </nav>
</template>

<script>
export default {
  name: 'Navigation',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
nav {
  display: flex;
  width: 100%;
  height: 50px;
  box-sizing: border-box;
  justify-content: space-between;
  padding: 10px;
  border-bottom: 1px solid lightgrey;
  align-items: center;
}

h2 {
  margin: 0;
  padding: 0 10px;
}

ul {
  display: flex;
  justify-content: space-between;
}

li {
  text-align: center;
  padding: 0 20px;
  cursor: pointer;
}

</style>
