<template>
  <div class="hello">
    <input type="text" class="gp-list" placeholder="Search..">
    <ul>
      <li v-for="listItem in listItems">{{ listItem }}</li>
    </ul>
  </div>
</template>

<script>
import data from "../../data/data.json";
let newData = data["shopping-carts"]["lisa"];
export default {
  data() {
    return {
      listItems: newData
    };
  }
};
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #35495e;
}
</style>
