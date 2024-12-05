<template>
  <div class="my_descr">
    * подробности в личных сообщениях на сайте. <a href="https://baltbet.ru/help/rules#common">Правила</a><br>
    БАЛТБЕТ букмекерская компания, 2003-2024 (ООО «Санторин») Информация об организаторе, правилах проведения акции, сроках, месте и порядке получения призов или выигрышей указана на сайте www.baltbet.ru
  </div>
</template>


<style lang="scss" scoped>
  .my_descr {
    text-align: left;
    text-transform: uppercase;
    font-size: 11.5px;
    color: #FFFFFF;

    & a {
      text-decoration: none;
      color: #FFFFFF;
      font-weight: 700;
    }
  }

  @media (max-width: 1200px) {
    .my_descr {
      font-size: 10px;
    }
  }

  @media (max-width: 992px) {
    .my_descr {
      font-size: 9px;
    }
  }

  @media (max-width: 576px) {
    .my_descr {
      text-align: center;
      font-size: 5px;
    }
  }
</style>