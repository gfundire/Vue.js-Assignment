<template>
  <section class="result-links center-flex">
    <span class="arrow"
      ><img src="../assets/l-arrow.svg" alt="previous page"
    /></span>
    <span>1</span>
    <span>2</span>
    <span>3</span>
    <span>4</span>
    <span>5</span>
    <span>6</span>
    <span>...</span>
    <span>13</span>
    <span class="arrow"
      ><img src="../assets/r-arrow.svg" alt="next page" />
    </span>
  </section>
</template>

<script>
  export default {
    name: "ResultLinks",
  };
</script>

<style scoped>
  .result-links {
    height: 50px;
    justify-content: space-evenly;
  }
  .arrow {
    color: #002d63;
    background-color: none;
  }
</style>
>
