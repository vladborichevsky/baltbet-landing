<template>
  <footer class="footer" id="footer">
    <div class="footer_icons">
      <div class="footer_icons_social">
        <a href="https://vk.com/bcavtodor" class="logo">
          <img src="/VK.svg" alt="VK_logo">
        </a>
        <a href="https://t.me/bcavtodor" class="logo">
          <img src="/telegram.svg" alt="telegram_logo">
        </a>
      </div>

      <second-button/>
      
      <div class="footer_icons_logos">
        <a href="https://baltbet.ru/" class="logo">
          <img src="/logo_bb.svg" alt="logo_baltbet">
        </a>
        <div class="footer_icons_logos_devider">x</div>
        <a href="https://avtodor.ru/" class="logo">
          <img class="avtotor_logo_img" src="/logo_avto.svg" alt="logo_avtodor">
        </a>
      </div>
    </div>

    <div class="footer_descr">
      <a href="Rules.pdf" download="">Полные правила можно прочитать тут</a>
      <p>Организатор конкурса СРМФСОО «Баскетбольный клуб «АВТОДОР»</p>
    </div>
  </footer>
</template>


<script setup>
  import SecondButton from '@/components/UI/SecondButton.vue'
</script>


<style lang="scss" scoped>
  .footer {
    margin: 20px 0;
    text-align: left;
    z-index: 1;
    padding-bottom: 10px;

    a {
      color: #ffff;
    }

    &_icons {
      display: flex;
      justify-content: space-between;
      align-items: center;

      &_social {
        width: 100px;
        display: flex;
        justify-content: space-between;

        img {
          width: 40px;
        }
      }

      &_logos {
        width: 250px;
        display: flex;
        justify-content: space-between;
        align-items: center;

        img {
          width: 100px;
          transform: translateY(3px);
        }
      }
    }

    &_descr {
      display: flex;
      justify-content: space-around;
      font-size: 12px;
      text-align: center;
      margin-top: 20px;
    }
  }

  @media (max-width: 767px) {
    .footer {
      a {
        font-size: 10px;
      }

      &_icons {
        margin-top: 0;

        &_social {
          width: 80px;

          img {
            width: 30px;
          }
        }

        &_logos {
          width: 150px;

          img {
            width: 60px;
          }
        }
      }

      &_descr {
        font-size: 10px;
        padding-bottom: 10px;
        display: block;
      }
    }
  }

  @media (max-width: 576px) {
    .footer {
      &_icons {
        display: block;

        &_social {
          margin: 0 auto;
          margin-bottom: 10px;
        }

        &_logos {
          margin: 0 auto;
          margin-top: 20px;

          .avtotor_logo_img {
            width: 40px;
          }
        }
      }

      &_descr {
        font-size: 10px;
        padding-bottom: 10px;
        display: block;
        margin-top: 5px;

        p {
          margin-top: 10px;
        }
      }
    }
  }
</style>