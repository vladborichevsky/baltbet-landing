<template>
  <div class="header">
    <div class="header_menu">
      <a href="#prizes">
        <button>призы</button>
      </a>
      <a href="#terms">
        <button>условия</button>
      </a>
      <a href="https://docs.google.com/forms/d/e/1FAIpQLSdQ8gL2cnjC6AxR9UgQUVwX3g9O_DDqY0c0_eWq85AjegTLqA/viewform">
        <button>подать заявку</button>
      </a>
      <a href="#footer">
        <button>контакты</button>
      </a>
    </div>

    <div class="header_logo">
      <a href="https://baltbet.ru/" class="logo">
        <img src="/logo_bb.svg" alt="logo_baltbet">
      </a>
      <div class="header_logo_devider">x</div>
      <a href="https://avtodor.ru/" class="logo">
        <img class="avtotor_logo_img" src="/logo_avto.svg" alt="logo_avtodor">
      </a>
    </div>
  </div>
</template>


<style lang="scss" scoped>
  @use '@/assets/variables' as vars;

  .header {
    width: 100%;
    display: flex;
    justify-content: space-between;
    margin: 0 auto;

    &_menu {
      width: 550px;
      display: flex;
      justify-content: space-between;
    }

    &_logo {
      display: flex;
      justify-content: space-between;
      align-items: center;
      width: 300px;
      z-index: 5;

      &_devider {
        color: #ffff;
      }

      img {
        width: 120px;
        cursor: pointer;
        transform: translateY(5px);
      }

      .avtotor_logo_img {
        width: 90px;
        transform: translateY(0);
      }
    }
  }

  button {
    cursor: pointer;
    height: fit-content;
    border: 1px #ffff solid;
    border-radius: 10px;
    font-size: 18px;
    line-height: 32px;
    padding: 0 20px;
    background-color: inherit;
    color: #ffff;
  }

  button:hover {
    background-color: vars.$orange-color;
    color: vars.$background-color;
    border: 1px vars.$orange-color solid;
    transition: all .5s;
  }

  @media (max-width: 1200px) {
    .header {
      align-items: center;

      &_menu {
        width: 450px;
      }

      &_logo {
        width: 200px;
        justify-content: space-between;
        align-items: center;
        height: fit-content;

        img {
          width: 80px;
          transform: translateY(3px);
        }
      }
    }

    button {
      font-size: 14px;
    }

    button:hover {
      background-color: inherit;
      color: #ffff;
      border: 1px #ffff solid;
    }
  }

  @media (max-width: 992px) {
    .header {
      &_menu {
        width: 400px;
      }
    }

    button {
      font-size: 12px;
      line-height: 32px;
      padding: 0 15px;
    }
  }

  @media (max-width: 767px) {
    .header {
      &_menu {
        width: 300px;
      }

      &_logo {
        width: 180px;

        img {
          width: 80px;
        }

        .avtotor_logo_img {
          width: 60px;
        }
      }
    }

    button {
      font-size: 10px;
      line-height: 25px;
      padding: 0 12px;
    }
  }

  @media (max-width: 576px) {
    .header {
      flex-direction: column;

      &_logo {
        margin-top: 15px;
        width: 180px;

        img {
          width: 60px;
          transform: translateY(0);
        }

        .avtotor_logo_img {
          width: 35px;
        }
      }
    }
  }
</style>