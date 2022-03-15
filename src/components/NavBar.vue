<script setup>
import { RouterLink } from "vue-router";
</script>

<template>
  <div class="sticky-wrapper">
    <nav>
      <ul>
        <li>
          <RouterLink to="/" active-class="active">MY FEED</RouterLink>
        </li>
        <li>
          <RouterLink to="/trends" active-class="active">TRENDS</RouterLink>
        </li>
        <li>
          <RouterLink to="/wallets" active-class="active"
            >CURATED WALLETS</RouterLink
          >
        </li>
        <li>
          <RouterLink to="/add" active-class="active">ADD WALLET</RouterLink>
        </li>
      </ul>
      <hr />
    </nav>
  </div>
</template>

<style scoped>
nav {
  background: #1e1e1e;
  height: 75px;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1;
}

.sticky-wrapper {
  height: 75px;
}
nav ul {
  list-style: none;
  padding: 0;
  margin: 0;
  text-align: center;
}
nav ul li {
  display: inline-block;
}
nav ul a {
  height: 65px;
  line-height: 65px;
  padding: 30px 0;
  margin: 0 25px;
  color: #a1a1a1;
  font-size: 20px;
  font-weight: 700;
  text-transform: uppercase;
  text-decoration: none;
}

nav ul a.active {
  box-shadow: 0 3px 3px -3px white;
  border-bottom: 3px solid white;
  color: white;
}
</style>
