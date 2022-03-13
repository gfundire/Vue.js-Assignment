<template>
  <header>
    <form action="" class="search-form">
      <button class="icon search-btn" type="submit">
        <img
          src="../assets/search.svg"
          alt="Search"
          width="15.09"
          height="16"
        />
      </button>

      <input id="location" type="search" placeholder="Search Location" />

      <input id="date" type="text" placeholder="Aug 18 -Aug 19" />
      <input
        id="guests"
        type="text"
        placeholder="2 adults, 1 room, 0 children"
      />
      <input class="search-btn" type="submit" value="Search" />
    </form>
  </header>
</template>

<script>
  export default {
    name: "HeaderComponent",
    props: {},
  };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  header {
    background: #ffffff;
    font-style: normal;
    font-weight: bold;
    font-size: 14px;
    line-height: 16px;
  }
</style>

<style>
  form input[type="submit"] {
    display: none;
  }

  form {
    display: grid;
    /* grid-auto-flow: column; */
    grid-template-columns: min-content 1fr 1fr;
    grid-template-rows: 30px 30px;
    height: 70px;
    padding: 0 1.2em;
    background: #ffffff;
    /* width: 90%; */
  }

  input {
    display: block;
  }

  .icon {
    grid-column: 1/2;
    grid-row: 1/3;
    background: #ffffff;
    border: none;
    justify-self: right;
    margin-right: 0.8em;
  }
  #location {
    grid-column: 2/4;
    grid-row: 1/2;
    font-weight: bold;
    font-size: 14px;
    line-height: 16px;
    color: #000000;
  }
  #guests {
    grid-column: 3/4;
    grid-row: 2/3;
  }

  #date,
  #guests {
    font-size: 12px;
    line-height: 16px;
    color: #333333;
  }
  input {
    border-style: none;
  }
</style>
