<template>
  <div class="rating">
    <div class="row spread center-flex">
      <span class="head">Star rating</span>
      <span class="clear-blue1">CLEAR</span>
    </div>
    <div class="row"><input type="checkbox" /><span>******</span></div>
    <div class="row"><input type="checkbox" /><span>****</span></div>
    <div class="row"><input type="checkbox" /><span>***</span></div>
    <div class="row"><input type="checkbox" /><span>**</span></div>
    <div class="row"><input type="checkbox" /><span>*</span></div>
  </div>
</template>
<script>
  export default {
    name: "StarRating",
  };
</script>
<style scoped>
  .head {
    font-weight: 700;
    font-size: 14px;
    line-height: 16px;
    color: #000000;
  }
  .row {
    height: 30px;
  }
  .rating {
    padding: 0 20px;
  }
</style>
