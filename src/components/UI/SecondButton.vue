<template>
  <div class="second_button_wrapper">
    <a class="second_button" href="https://docs.google.com/forms/d/e/1FAIpQLSdQ8gL2cnjC6AxR9UgQUVwX3g9O_DDqY0c0_eWq85AjegTLqA/viewform">
      <span>ОТПРАВИТЬ ИДЕЮ ДИЗАЙНА</span>
    </a>
</div>
</template>


<style lang="scss" scoped>
  @use '@/assets/variables' as vars;

  .second_button_wrapper {
    width: fit-content;
  }

  .second_button {
    border-radius: 10px;
    display: flex;
    padding: 10px 45px;
    text-decoration: none;
    font-size: 30px;
    color: white;
    background: vars.$orange-color;
    transition: 1s;
    box-shadow: 10px 10px 0 black;
    transform: skewX(-15deg);
    line-height: 30px;
    font-weight: 700;
  }

  .second_button:focus {
    outline: none; 
  }

  .second_button:hover {
    transition: 0.5s;
    box-shadow: 10px 10px 0 #FBC638;
  }

  span {
    height: 32px;
    transform: skewX(15deg);
    line-height: 32px;
  }

/* SVG animations */

  @keyframes color_anim {
    0% {
        fill: white;
    }
    50% {
        fill: #FBC638;
    }
    100% {
        fill: white;
    }
  }

  @media (max-width: 1200px) {
    .second_button {
      padding: 10px 35px;
      font-size: 25px;
      line-height: 25px;
    }

    .second_button:hover {
      box-shadow: 10px 10px 0 black;
    }
  }

  @media (max-width: 992px) {
    .second_button {
      padding: 10px 15px;
      font-size: 18px;
      line-height: 18px;
    }
  }

  @media (max-width: 767px) {
    .second_button {
      padding: 5px 12px;
      font-size: 14px;
      line-height: 14px;
    }
  }

  @media (max-width: 576px) {
    .second_button_wrapper {
      margin: 0 auto;
    }
  }
</style>