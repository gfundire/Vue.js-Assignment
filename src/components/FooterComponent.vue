<template>
  <footer>
    <div class="contacts">
      <ul class="center-flex">
        <li><a>FAQ</a></li>
        <li><a>Terms of use</a></li>
        <li><a>Privacy policy</a></li>
        <li><a>Contact us</a></li>
      </ul>
    </div>
    <div class="credits center-flex">&copy; CloudTravel 2021</div>
  </footer>
</template>

<script>
  export default {
    name: "FooterComponent",
  };
</script>

<style scoped>
  footer {
    color: #ffffff;
  }
  .contacts {
    background: #333333;
    height: 50px;
  }

  .credits {
    background-color: #000000;
    font-style: normal;
    font-weight: normal;
    font-size: 10px;
    line-height: 13px;
    height: 30px;
    justify-content: center;
  }

  .contacts ul {
    display: flex;
    height: inherit;
    align-items: center;
    justify-content: space-evenly;
  }
</style>
