<script setup>
import IconChevronRight from "./icons/IconChevronRight.vue";

defineProps({
  item: {
    type: Object,
    required: true,
  },
});
</script>

<template>
  <div class="post">
    <div class="post__top">
      <div class="post__top-left">
        <img class="post__profile-img" :src="item.picture" alt="" />
        <div class="post__content">
          <p class="post__profile-name">{{ item.name }}</p>
          <div>
            <p class="p">{{ item.address }}</p>
            <p class="p">{{ item.date }}</p>
          </div>
        </div>
      </div>
      <div class="post__top-right">
        <button class="bubble">{{ item.state }}</button>
        <button class="bubble balance">{{ item.balance }}</button>
        <span class="post__date-posted">{{ item.timestamp }}</span>
        <button class="bubble next">
          <IconChevronRight />
        </button>
      </div>
    </div>
  </div>
</template>

<style scoped>
.post {
  width: 100%;
  background-color: #0f0f0f;
  margin: 0 auto;
  min-height: 100px;
  border-radius: 3px;
  padding: 12px 18px;
  clip-path: polygon(3% 0%, 100% 0, 100% 73%, 97% 100%, 0 97%, 0 22%);
}

.post__top {
  margin: 0 40px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.post__top-left {
  display: flex;
  align-items: center;
}

.post__profile-img {
  height: 70px;
  width: 70px;
  border-radius: 50%;
  object-fit: cover;
  margin-right: 10px;
}

.post__profile-name {
  color: white;
  text-decoration: none;
  font-size: 16px;
  margin-bottom: 6px;
}

.post__date-posted {
  font-size: 16px;
  color: #797979;
  font-family: "Graphik";
}

/* Content */
.post__content {
  padding: 14px 8px;
}
.p {
  font-size: 14px;
  color: #797979;
  font-family: "Graphik";
}

.bubble {
  background-color: #ff0000;
  border: none;
  color: white;
  padding: 10px 24px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-weight: bold;
  font-size: 16px;
  font-family: "Graphik", Helvetica, Arial;
  margin: 4px 2px;
  border-radius: 25px;
  margin-right: 12px;
}

.balance {
  background: transparent;
  border: 1px solid #232323;
}

.next {
  margin-left: 48px;
  padding: 13px;
  background: #242424;
  border-radius: 50%;
  place-items: center;
  cursor: pointer;
  width: 40px;
  height: 40px;
}
</style>
