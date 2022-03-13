<template>
  <div class="container">
    <div class="filter center-flex">
      <img src="../assets/x-close.svg" alt="close" />
      <span>Sort & Filter</span>
    </div>
    <div class="ht grey filter center-flex">Sort By</div>
    <div class="dp-down spread ht center-flex">
      Price (lowest first)
      <select name="" id=""></select>
    </div>
    <div class="ht grey filter center-flex">Filter by</div>
    <div class="price">
      <div class="spread row center-flex">
        <span class="head">Price per night</span
        ><span class="clear-blue1">CLEAR</span>
      </div>
      <input type="range" min="0" max="550" />
      <div class="sgd spread row center-flex">
        <input type="text" value="SGD 0" />
        -
        <input type="text" value="SGD 550" />
      </div>
    </div>
    <reviews-component />
    <star-rating />
    <div class="fix spread filter center-flex">
      <input id="clear-btn" type="button" value="Clear" />
      <input id="filter-btn" type="button" value="Filter" />
    </div>
  </div>
</template>
<script>
  import ReviewsComponent from "./ReviewsComponent.vue";
  import StarRating from "./StarRating.vue";
  export default {
    name: "FilterComponent",
    components: {
      ReviewsComponent,
      StarRating,
    },
  };
</script>
<style scoped>
  .container {
    background: #ffffff;
    min-height: 100vh;
  }
  .filter {
    height: 50px;
    background: #ffffff;
    border-bottom: 1px solid #dddddd;
    font-weight: 700;
    font-size: 16px;
    line-height: 20px;
    color: #002d63;
  }
  .filter span,
  .flter img {
    margin-left: 20px;
  }
  .ht {
    height: 40px;
  }
  .grey {
    background: #f5f5f5;
  }
  .fix {
    height: 60px;
    position: sticky;
    bottom: 0;
    border-top: 1px solid #dddddd;
  }

  .row {
    height: 50px;
  }

  .price {
    display: flex;
    flex-direction: column;
  }

  input[type="text"] {
    background: #ffffff;
    border: 1px solid #dddddd;
    border-radius: 3px;
    height: 30px;
  }
  range,
  .price,
  .filter,
  .dp-down {
    padding: 0 20px;
  }

  #clear-btn {
    color: #002d63;
    background: #ffffff;
  }
  #filter-btn {
    color: #ffffff;
    background: #002d63;
  }
  #clear-btn,
  #filter-btn {
    width: 177px;
    height: 40px;
    font-weight: 700;
    font-size: 14px;
    line-height: 18px;
    border: 1px solid #002d63;
    border-radius: 3px;
  }
</style>
