<template>
  <div class="main_info">
    <div class="main_info_text">
      <p>
        Мы ценим наши отношения<br>
        и предлагаем вам<br>
        эксклюзивный бонус:
      </p>
      <br>
      <p class="light">
        Пройдите приветственные задания<br>
        и получите фрибет 600 руб.
      </p>

      <img src="/devidor.svg" alt="">

      <p>
        После прохождения<br>
        получите запас ставок 1000 руб.
      </p>
    </div>

    <main-button/>
  </div>
</template>

<script setup>
  import MainButton from '@/components/MainButton.vue'
</script>

<style lang="scss" scoped>
  .main_info {
    margin-top: 40px;
    display: flex;
    justify-content: space-between;
    align-items: end;

    &_text {
      color: #ffff;
      font-size: 23px;
      text-transform: uppercase;
      text-align: left;
      text-shadow: rgba(4, 25, 255, 0.988) 1px 1px 10px;
      font-weight: 700;
    }
  }

  .light {
    font-weight: 300;
  }

  @media (max-width: 1200px) {
    .main_info_text {
      font-size: 20px;

      & img {
        width: 400px;
      }
    }
  }

  @media (max-width: 992px) {
    .main_info_text {
      font-size: 18px;

      & img {
        width: 300px;
      }
    }
  }

  @media (max-width: 767px) {
    .main_info_text {
      font-size: 16px;

      & img {
        width: 250px;
      }
    }
  }

  @media (max-width: 576px) {
    .main_info {
      flex-direction: column;
      align-items: center;
      transform: translateY(30%);
    }

    .main_info_text {
      font-size: 12px;
      text-align: center;
      
      & img {
        width: 220px;
      }
    }
  }
</style>