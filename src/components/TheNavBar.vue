<script>
// importo l'array
import { menuItems } from "../composable/navBarItems";
export default {
  data() {
    return {

      menuItems: menuItems,
      
    };
  },
  methods: {},
};
</script>

<template>
  <div class="container">
    <nav class="d-flex justify-content-between align-items-center">
      <div class="logoNav">
        <img src="../assets/dc-logo.png" alt="" />
      </div>
      <div class="menunav">
        <ul>
          <li v-for="itemsNavBar in menuItems">
            <a href="#">{{ itemsNavBar }}</a>
          </li>
        </ul>
      </div>
    </nav>
  </div>
</template>

<style scoped>
img {
  width: 80px;
  aspect-ratio: 1/1;
  margin: 10px 0px;
}

ul {
  display: flex;
  list-style: none;
  gap: 40px;
  margin-bottom: 0px;
}

li {
  padding: 35px 0;
}

li:hover {
  border-bottom: 5px solid #157df0;
}

a {
  text-decoration: none;
  color: grey;
}

a:hover {
  color: #157df0;
}
</style>
