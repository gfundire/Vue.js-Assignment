<template>
  <nav-component />
  <header-component />
  <search-bar />
  <sort-filter />
  <filter-component />
  <!-- <results-count />
  <result-links /> -->
  <!-- <footer-component /> -->
</template>

<script>
  import NavComponent from "./components/NavComponent.vue";
  // import HeaderComponent from "./components/HeaderComponent.vue";
  // import PropertyComponent from "./components/PropertyComponent.vue";
  // import ResultsCount from "./components/ResultsCount.vue";
  // import ResultLinks from "./components/ResultLinks.vue";
  import SearchBar from "./components/SearchBar.vue";
  // import SortFilter from "./components/SortFilter.vue";
  // import FilterComponent from "./components/FilterComponent.vue";
  // import FooterComponent from "./components/FooterComponent.vue";

  export default {
    name: "App",
    components: {
      NavComponent,
      // HeaderComponent,
      // SortFilter,
      SearchBar,
      // FilterComponent,
      // ResultsCount,
      // ResultLinks,
      // FooterComponent,
    },
  };
</script>

<style>
  /* Box sizing */
  html {
    box-sizing: border-box;
  }
  *,
  *:before,
  *:after {
    box-sizing: inherit;
  }
  /* reset */
  html,
  body {
    margin: 0;
    padding: 0;
    /* width: 100vw;  */
    font-family: Mulish, Avenir, Helvetica, Arial, sans-serif;
    font-style: normal;
    font-weight: normal;
    background: #e5e5e5;
    min-height: 100vh;
    color: #000000;
    display: grid;
    grid-template-columns: 1fr;
  }

  nav li,
  footer li {
    list-style-type: none;
  }
  a {
    text-decoration: none;
  }
  ul {
    margin: 0;
    padding: 0;
  }

  .center-flex {
    display: flex;
    align-items: center;
  }
  .spread {
    justify-content: space-between;
  }
  .head {
    font-weight: 700;
    font-size: 14px;
    line-height: 16px;
    color: #000000;
  }
  .clear-blue1 {
    color: #002d63;
    font-weight: 700;
    font-size: 12px;
    line-height: 20px;
  }
</style>
