<script setup>
import CustomCard from "./CustomCard.vue";

const data = [
  {
    name: "X Rabbitars",
    address: "0x6...d82",
    date: "21.10.22 20:24",
    state: "Sold",
    balance: "0.188 ETH",
    timestamp: "1h 30min",
    picture:
      "https://media.playboyrabbitars.com/images/rabbitars/RARE_HARE_5.jpg",
  },
  {
    name: "X Rabbitars",
    address: "0x6...d82",
    date: "21.10.22 20:24",
    state: "Sold",
    balance: "0.188 ETH",
    timestamp: "1h 30min",
    picture:
      "https://media.playboyrabbitars.com/images/rabbitars/RARE_HARE_6.jpg",
  },
  {
    name: "X Rabbitars",
    address: "0x6...d82",
    date: "21.10.22 20:24",
    state: "Sold",
    balance: "0.188 ETH",
    timestamp: "1h 30min",
    picture:
      "https://media.playboyrabbitars.com/images/rabbitars/RARE_HARE_10.jpg",
  },
  {
    name: "X Rabbitars",
    address: "0x6...d82",
    date: "21.10.22 20:24",
    state: "Sold",
    balance: "0.188 ETH",
    timestamp: "1h 30min",
    picture:
      "https://media.playboyrabbitars.com/images/rabbitars/RARE_HARE_3.jpg",
  },
  {
    name: "X Rabbitars",
    address: "0x6...d82",
    date: "21.10.22 20:24",
    state: "Sold",
    balance: "0.188 ETH",
    timestamp: "1h 30min",
    picture:
      "https://media.playboyrabbitars.com/images/rabbitars/RARE_HARE_1.jpg",
  },
];
</script>

<template>
  <div class="feed">
    <CustomCard v-for="(item, index) in data" :key="index" :item="item" />
  </div>
</template>

<style scoped>
.feed {
  margin: 0 auto;
  width: 80%;
  position: relative;
}
</style>
