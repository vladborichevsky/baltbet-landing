<template>
  <div class="main_info_conteiner">
    <div class="main_info">
      <h1>СОЗДАЙ <span>НОВУЮ ФОРМУ</span> ДЛЯ ЛЮБИМОЙ КОМАНДЫ И <span>ПОЛУЧИ ПРИЗ</span></h1>
      <div class="main_info_subtitle">Для участия необязательны графические редакторы, главное – идея!</div>
      <main-button/>
      <div class="main_info_deadline">Заявки принимаются <span>до 15 января</span></div>
      <div class="main_info_descr">
        <img src="/thunder.svg" alt="thunder">
        <p>Прими участие в создании дизайна новой формы для баскетбольного клуба «Автодор» в ЕЛ ВТБ и получи <span>денежный приз!</span>
        </p>
      </div>
    </div>
    <div class="main_info_img">
      <img src="/player.png" alt="player">
    </div>
  </div>
</template>


<script setup>
  import MainButton from '@/components/UI/MainButton.vue'
</script>


<style lang="scss" scoped>
  @use '@/assets/variables' as vars;

  .main_info_conteiner {
    margin: 0 auto;
    display: flex;
    align-items: center;
    text-align: left;
  }

  h1 {
    margin-bottom: 15px;
    line-height: 50px;
    font-size: 50px;

    span {
      color: vars.$orange-color;
    }
  }

  .main_info {
    width: 50%;
    z-index: 5;

    &_subtitle {
      margin: 15px 0;
    }

    &_deadline {
      margin: 15px 0;

      span {
        font-weight: 700;
      }
    }

    &_descr {
      display: flex;
      align-items: center;
      position: relative;
      left: -65px;

      img {
        width: 130px;
      }

      p {
        font-size: 20px;
        line-height: 20px;
      }

      span {
        color: vars.$orange-color;
        font-weight: 700;
      }
    }

    &_img {
      z-index: -1;
      width: 500px;
      height: 100%;

      img {
        width: 500px;
        height: 100%;
      }
    }
  }

  @media (max-width: 1200px) {
    .main_info {
      &_img {
        width: 400px;

        img {
          width: 400px;
        }
      }

      &_descr {
        left: 0;
      }
    }
  }

  @media (max-width: 992px) {
    h1 {
      margin-bottom: 10px;
      line-height: 30px;
      font-size: 30px;
    }

    .main_info {
      &_subtitle {
        margin: 10px 0;
      }

      &_deadline {
        margin: 10px 0;
      }

      &_descr {
        margin: 10px 0;

        img {
          width: 110px;
        }

        p {
          font-size: 16px;
        }
      }
    }
  }

  @media (max-width: 767px) {
    h1 {
      margin-bottom: 10px;
      line-height: 25px;
      font-size: 22px;
    }

    .main_info {
      &_subtitle {
        font-size: 12px;
      }

      &_img {
        width: 350px;

        img {
          width: 350px;
        }
      }

      &_descr {
        margin: 0;
        left: -40px;
        
        p {
          font-size: 12px;
          line-height: 12px;
        }

        img {
          width: 80px;
        }
      }
    }
  }

  @media (max-width: 576px) {
    h1 {
      line-height: 25px;
      font-size: 25px;
    }

    .main_info {
      padding-left: 15px;
      width: 50%;

      &_subtitle {
        font-size: 14px;
      }

      &_deadline {
        font-size: 14px;
      }

      &_img {
        width: 250px;
        overflow: hidden;

        img {
          width: 175%;
        }
      }

      &_descr {
        width: 120%;
        transform: translateX(10%);
        margin-top: 20px;
        
        p {
          font-size: 18px;
          line-height: 18px;
        }

        img {
          width: 50px;
        }
      }
    }
  }

  @media (max-width: 500px) {
    h1 {
      line-height: 22px;
      font-size: 22px;
    }

    .main_info_descr {
      p {
        font-size: 14px;
        line-height: 14px;
      }
    }
  }

  @media (max-width: 440px) {
    h1 {
      line-height: 18px;
      font-size: 18px;
    }

    .main_info_descr {
      p {
        font-size: 12px;
        line-height: 12px;
      }
    }
  }
  
  @media (max-width: 340px) {
    h1 {
      line-height: 11px;
      font-size: 11px;
    }

    .main_info {
      padding-left: 15px;
      width: 50%;

      &_subtitle {
        font-size: 9px;
      }

      &_deadline {
        font-size: 10px;
      }

      &_img {
        width: 250px;
        overflow: hidden;

        img {
          width: 175%;
        }
      }

      &_descr {
        width: 150%;
        transform: translateX(10%);
        margin-top: 20px;
        
        p {
          font-size: 10px;
        }

        img {
          width: 50px;
        }
      }
    }
  }
</style>