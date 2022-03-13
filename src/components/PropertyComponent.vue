<template>
  <article>
    <img src="" alt="" />
    <div>
      <h1>{{ title }}</h1>
      <div>
        <img :src="imgUrl" :alt="title" />
      </div>

      <address>
        80 Collyer quay, Marina Bay, Singapore, Singapore, 049326
      </address>
      (<a href="#">view map</a>)

      <div class="promo">
        <div class="disc">SAVE {{ disc }}% TODAY</div>
        <p>Nightly avg</p>
        {{ currency + initialPrice }} <strong>SGD 100</strong>
      </div>
    </div>
  </article>
  <results-count />
  <result-links />
</template>
<script>
  import ResultsCount from "./ResultsCount.vue";
  import ResultLinks from "./ResultLinks.vue";
  export default {
    name: "PropertyComponent",
    components: {
      ResultsCount,
      ResultLinks,
    },
    data() {
      return {
        title: "The Fulleton Bay Hotel",
        disc: 16,
        stars: 4.5,
        currentPrice: 100,
        initialPrice: 120,
        currency: "SGD ",
        imgUrl: "../assets/fullerton.png",
      };
    },
  };
</script>

<style>
  article {
    font-weight: bold;
    font-size: 14px;
    line-height: 16px;
    color: #333333;
    width: 80%;
    margin: 0 auto;
  }
</style>
