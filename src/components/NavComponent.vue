<template>
  <nav class="center-flex">
    <div class="wrapper center-flex">
      <section class="logo">
        <a href="#">
          <img
            src="../assets/cloudtravel-logo.svg"
            alt="CloudTravel"
            width="162.5"
            height="25"
          />
        </a>
      </section>
      <button class="hamburger">
        <img src="../assets/hamburger.svg" alt="view links" width="18.75" />
      </button>
    </div>
    <section class="menu">
      <ul class="links">
        <li><a href="#" id="language">English</a></li>
        <li><a href="#" id="currency">USD</a></li>
        <li><a href="#" id="account">My&nbsp;Account</a></li>
        <li><a href="#">Logout</a></li>
      </ul>
    </section>
  </nav>
</template>

<script>
  export default {
    name: "NavComponent",
    props: {},
  };
</script>

<style scoped>
  nav {
    font-style: normal;
    font-weight: normal;
    font-size: 12px;
    line-height: 16px;
    color: #333333;
    padding: 0 5%;
    background-color: #ffffff;
    border-bottom: 2px solid #e5e5e5;
  }

  .wrapper {
    height: 60px;
    width: 100%;
    justify-content: space-between;
  }

  .hamburger {
    justify-self: right;
    background-color: #ffffff;
    border: none;
    margin-right: -4px;
  }

  #language,
  #account {
    background-color: #e5e5e5;
  }

  .links a {
    color: #333333;
    display: block;
    padding: 0.5em;
  }

  /* Hide Menu */
  .menu {
    display: none;
  }
  @media screen and (min-width: 990px) {
    .menu {
      display: block;
    }
    .hamburger {
      display: none;
    }
    nav {
      display: flex;
      height: 60px;
    }
    .links {
      display: flex;
    }
    .links a {
      display: inline;
      padding: 0 0.8em;
    }
    #language,
    #account {
      background-color: #ffffff;
    }
  }
</style>
