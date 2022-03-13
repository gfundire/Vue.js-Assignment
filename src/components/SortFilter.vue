<template>
  <section id="top" class="sort-filter">
    <div class="col-2">
      <div id="sort">Sort & Filter</div>
      <div id="map-view" class="center-flex">
        <span><img src="../assets/location.svg" alt="Map View" /></span>
        <span>Map View</span>
      </div>
    </div>
    <div class="select">
      <select>
        <option value="">Select One</option>
      </select>
    </div>
    <h4>Singapore: 9999 properties found</h4>
    <div class="results-area">
      <property-component />
    </div>
  </section>
</template>

<script>
  import PropertyComponent from "./PropertyComponent.vue";
  export default {
    name: "SortFilter",
    components: {
      PropertyComponent,
    },
  };
</script>

<style scoped>
  .col-2,
  .select {
    height: 60px;
  }
  .col-2 {
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    /* border-bottom: 2px solid #e5e5e5; */
  }

  .sort-filter {
    font-size: 14px;
    line-height: 20px;
    color: #002d63;
    border-top: 2px solid #e5e5e5;
    background-color: #ffffff;
  }
  .sort-filter img {
    margin-right: 1em;
    padding-top: 0.25em;
    /* border-top: 2px solid #e5e5e5; */
  }
  .results-area {
    min-height: 100vh;
  }
  h4 {
    text-align: center;
    font-weight: bold;
    font-size: 14px;
    line-height: 16px;
    color: #000000;
  }

  .select {
    margin: 0.5em 0;
    text-align: left;
    height: 30px;
    display: flex;
    justify-content: center;
  }
  .select select {
    width: 80%;
    background-color: #002d63;
    color: #ffffff;
    font-weight: bold;
    font-size: 14px;
    line-height: 16px;
    border-radius: 3px;
  }
</style>
