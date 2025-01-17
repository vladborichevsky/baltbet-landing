<template>
  <button @click="openLink()">
    забрать бонус
  </button>
</template>

<script setup>
  const openLink = () => {
    window.open("https://baltbet.ru/account/register")
  }
</script>

<style lang="scss" scoped>
  button {
    width: 300px;
    cursor: pointer;
    margin-right: 150px;
    height: 65px;
    border-radius: 25px;
    border: none;
    text-transform: uppercase;
    padding: 15px 20px;
    font-size: 30px;
    font-weight: 700;
    background: rgb(221,184,50);
    background: linear-gradient(121.59deg, #D9A317 20.59%, #FFE585 41%, #FBBC21 74.68%, #EFBD3E 87.76%, #D9A317 99.08%);
    animation-name: transformScale;
    animation-duration: 2s;
    animation-iteration-count: infinite;
    animation-timing-function: ease;
                
    &:hover {
      background: rgb(163,136,38);
      background: linear-gradient(121.59deg, #E4A90E 46.1%, #FFE585 62.97%, #FBBC21 77.89%, #EFBD3E 89.66%, #D9A317 99.08%);
      animation-play-state: paused;
    }
  }

  @media (max-width: 1200px) {
    button {
      width: 250px;
      margin-right: 65px;
      font-size: 25px;
    }
  }

  @media (max-width: 992px) {
    button {
      width: 220px;
      margin-right: 20px;
      font-size: 20px;
      padding: 10px 15px;

      &:hover {
        background: rgb(221,184,50);
        background: linear-gradient(121.59deg, #D9A317 20.59%, #FFE585 41%, #FBBC21 74.68%, #EFBD3E 87.76%, #D9A317 99.08%);
      }
    }
  }

  @media (max-width: 767px) {
    button {
      width: 200px;
      height: 50px;
      margin-right: 10px;
      font-size: 18px;
      padding: 5px 10px;
    }
  }

  @media (max-width: 576px) {
    button {
      width: 190px;
      height: 40px;
      margin-top: 10px;
      margin-right: 0;
      font-size: 18px;
      padding: 5px 10px;
    }
  }

  @keyframes transformScale {
    from {transform: scale(1)}
    50% {transform: scale(1.1)}
    to {transform: scale(1)}
  }
</style>