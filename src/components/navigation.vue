<template>
  <nav>
    <ul>
      <li>Create</li>
      <li>Edit</li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
nav {
  width: 100%;
  display: flex;
}

ul {
  display: flex;
  width: 200px;
  margin: 0;
  padding: 10px;
  justify-content: space-between;
  list-style-type: none;
}

</style>
