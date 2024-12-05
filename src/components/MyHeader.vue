<template>
  <div class="my_header">
    <a href="https://baltbet.ru/account/register" class="logo">
      <img src="/bb_logo.svg" alt="logo">
    </a>

    <img src="/18+.svg" alt="logo">
  </div>
</template>


<style lang="scss" scoped>
  .my_header {
    width: 100%;
    display: flex;
    justify-content: space-between;

    & a {
      display: block;
    }

    & a img {
      width: 200px;
    }
  }

  @media (max-width: 576px) {
    .my_header {
      margin-top: 10px;

      & a img {
        width: 100px;
      }

      & img {
        width: 20px;
      }
    }
  }
</style>