<template>
  <div class="reviews">
    <div class="row spread center-flex">
      <span class="head">Reviews</span><span class="clear-blue1">CLEAR</span>
    </div>
    <div class="row spread center-flex">
      <label for=""><input type="checkbox" />Excellent </label>
      <span>999</span>
    </div>
    <div class="row spread center-flex">
      <label for=""><input type="checkbox" />Very Good </label><span>999</span>
    </div>
    <div class="row spread center-flex">
      <label for=""><input type="checkbox" /> Good</label><span>999</span>
    </div>
    <div class="row spread center-flex">
      <label for=""><input type="checkbox" />Fair </label><span>999</span>
    </div>
    <div class="row spread center-flex">
      <label for=""><input type="checkbox" />Poor </label><span>999</span>
    </div>
    <div class="row spread center-flex">
      <label for=""><input type="checkbox" />No review </label><span>999</span>
    </div>
  </div>
</template>
<script>
  export default {
    name: "ReviewsComponent",
  };
</script>
<style scoped>
  .row {
    height: 30px;
  }
  .head {
    font-weight: 700;
    font-size: 14px;
    line-height: 16px;
    color: #000000;
  }
  .reviews {
    padding: 0 20px;
  }
</style>
