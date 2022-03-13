<template>
  <div class="where center-flex">
    <img src="../assets/x-close.svg" alt="close" />
    <span>Where?</span>
  </div>
  <form action="">
    <div class="container">
      <input id="location" type="text" placeholder="Singapore, Singapore" />
      <input id="date" type="text" placeholder="Jul 19  –  Jul 20" />
      <input
        id="guests"
        type="text"
        placeholder="2 adults, 0 children, 1 room"
      />
      <input id="search" type="submit" value="Search" />
    </div>
  </form>
</template>
<script>
  export default {
    name: "SearchBar",
  };
</script>

<style>
  form {
    background: #ffffff;
    /* height: 100vh; */
    padding: 0 20px;
    font-weight: 400;
    font-size: 14px;
    line-height: 20px;
  }
  .where {
    height: 50px;
    background: #ffffff;
    border-bottom: 1px solid #dddddd;
    font-weight: 700;
    font-size: 16px;
    line-height: 20px;
    color: #002d63;
  }
  .where span,
  .where img {
    margin-left: 20px;
  }
  input {
    height: 40px;
    width: 100%;
    margin-top: 20px;
    border: 1px solid #dddddd;
    border-radius: 3px;
    padding-left: 10px;
  }
  input[type="submit"] {
    width: 50%;
    background: #00a1e6;
    color: #ffffff;
    border: 1px solid #00a1e6;
    border-radius: 3px;
    font-weight: 700;
    font-size: 14px;
    line-height: 18px;
    padding-left: 0;
  }
  /* Tablet */
  @media screen and (min-width: 500px) {
    .container {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 10px;
    }
    input[type="submit"] {
      width: 100%;
    }
  }
  /* Desktop */
  @media screen and (min-width: 990px) {
    .container {
      width: 100vw;
      display: grid;
      grid-template-columns: repeat(12, 1fr);
      grid-template-rows: 1/2;
      grid-auto-flow: column;
      gap: 10px;
      padding: 0 4rem;
      background-color: #002d63;
      height: 70px;
      border-radius: 3px;
      position: sticky;
      top: 0;
    }
    div.where {
      display: none;
    }
    #location {
      grid-column: span 4;
    }
    #date,
    #guests {
      grid-column: span 3;
    }
    #search {
      grid-column: 11/13;
    }
    input {
      align-self: center;
      margin-top: 0;
    }
    input[type="submit"] {
      width: 100%;
    }
    form {
      padding: 0;
    }
  }

  .display-area {
    height: 100%;
    background: palevioletred;
    display: grid;
    grid-template-columns: repeat(12, 1fr);
  }
</style>
