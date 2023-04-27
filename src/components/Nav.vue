<template>
  <div class="nav">
    <router-link to="/money"
                 class="icon"
                 active-class="selected">
      <img class="orange-img" src="@/assets/money-orange.svg" alt="">
      <img class="black-img" src="@/assets/money.svg" alt="">
      <div class="icon-font">记账</div>
    </router-link>

    <router-link to="/labels"
                 class="icon"
                 active-class="selected">
      <img class="orange-img" src="@/assets/label-orange.svg" alt="">
      <img class="black-img" src="@/assets/label.svg" alt="">
      <div class="icon-font">标签</div>
    </router-link>

    <router-link to="/statistics"
                 class="icon"
                 active-class="selected">
      <img class="orange-img" src="@/assets/statistics-orange.svg" alt="">
      <img class="black-img" src="@/assets/statistics.svg" alt="">
      <div class="icon-font">统计</div>
    </router-link>
  </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
.nav {
  display: flex;
  justify-content: space-around;
  box-shadow: 0 0 3px rgba(0, 0, 0, .25);
  padding: 2px 0;

  .icon {
    display: flex;
    flex-direction: column;
    align-items: center;

    img {
      width: 32px;
      height: 32px;
      margin-bottom: 2px;
    }

    .orange-img {
      display: none;
    }

    .icon-font {
      font-size: 12px;
    }
  }

  .selected {
    .orange-img {
      display: block;
    }

    .black-img {
      display: none;
    }

    .icon-font {
      color: #ff6600;
    }
  }
}
</style>