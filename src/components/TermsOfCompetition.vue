<template>
  <div class="terms" id="terms">
    <div>
      <h2>УСЛОВИЯ КОНКУРСА</h2>
      <div class="terms_descr">
        Поделись своей идеей — <span>нарисуй форму в графическом редакторе или на бумаге</span> и загрузи заявку.<br><br>
        Выбирать победителей будет жюри из игроков и тренеров команды, менеджмента «Автодора» и «Балтбета».
      </div>
    </div>
    <img src="/versus.png" alt="versus_image">
  </div>
</template>


<style lang="scss" scoped>
  @use '@/assets/variables' as vars;

  h2 {
    font-size: 32px;
    text-align: left;
    margin-bottom: 20px;
  }

  .terms {
    margin: 0 auto;
    margin-top: 20px;
    display: flex;
    justify-content: center;
    align-items: center;

    &_descr {
      width: 750px;
      text-align: left;
      font-size: 22px;

      span {
        color: vars.$orange-color;
        font-weight: 700;
      }
    }

    img {
      width: 300px;
      height: 100%;
    }
  }
 
  @media (max-width: 1200px) {
    .terms {
      img {
        width: 250px;
      }

      &_descr {
        width: 600px;
        text-align: left;
        font-size: 20px;
        line-height: 20px;
      }
    }
  }

  @media (max-width: 992px) {
    .terms {
      margin-top: 20px;

      &_descr {
        width: 500px;
      }

      img {
        width: 200px;
      }
    }
  }

  @media (max-width: 767px) {
    h2 {
      font-size: 20px;
      margin-bottom: 0;
    }

    .terms {
      margin-top: 0;

      &_descr {
        width: 360px;
        font-size: 16px;
      }

      img {
        width: 130px;
      }
    }
  }

  @media (max-width: 576px) {
    h2 {
      font-size: 14px;
    }

    .terms {
      margin-top: 10px;
      padding: 0 20px;

      &_descr {
        width: 80%;
        font-size: 11px;
        line-height: 11px;
      }

      img {
        width: 100px;
      }
    }
  }
</style>