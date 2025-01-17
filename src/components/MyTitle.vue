<template>
  <div class="my_title">
    Специальное<br>
    предложение!
  </div>
</template>


<style lang="scss" scoped>
  .my_title {
    margin-top: 40px;
    text-align: left;
    text-transform: uppercase;
    font-weight: 900;
    font-size: 55px;
    line-height: 60px;
    text-underline-position: from-font;
    text-decoration-skip-ink: none;
    background: linear-gradient(121.59deg, #D9A317 20.59%, #FFE585 41%, #FBBC21 74.68%, #EFBD3E 87.76%, #D9A317 99.08%);
    background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  @media (max-width: 1200px) {
    .my_title {
      margin-top: 15px;
      font-size: 40px;
      line-height: 40px;
    }
  }

  @media (max-width: 992px) {
    .my_title {
      margin-top: 0;
      font-size: 30px;
      line-height: 30px;
    }
  }

  @media (max-width: 767px) {
    .my_title {
      font-size: 25px;
      line-height: 25px;
    }
  }

  @media (max-width: 576px) {
    .my_title {
      transform: translateY(-60%);
      text-align: center;
      font-size: 30px;
      line-height: 30px;
    }
  }
</style>

