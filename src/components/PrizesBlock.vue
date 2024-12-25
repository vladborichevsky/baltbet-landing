<template>
  <div class="prizes_block" id="prizes">
    <div class="prizes_block_first_line">
      <img src="/1_place.png" alt="prize_image">
      <img src="/2_place.png" alt="prize_image">
      <img src="/3_place.png" alt="prize_image">
    </div>
    <img class="prizes_block_second_line" src="/season_pass.svg" alt="season_pass">
  </div>
</template>


<style lang="scss" scoped>
  .prizes_block {
    &_first_line {
      margin: 0 auto;
      display: flex;
      justify-content: center;

      img {
        width: 300px;
      }
    }

    &_second_line {
      position: relative;
      width: 55%;
      z-index: -5;
    }
  }

  @media (max-width: 1200px) {
      .prizes_block {
        &_first_line {
          img {
            width: 250px;
          }
        }
      }
    }

  @media (max-width: 992px) {
    .prizes_block {
      &_first_line {
        img {
          width: 200px;
        }
      }
    }
  }

  @media (max-width: 767px) {
    .prizes_block {
      &_first_line {
          margin-top: 20px;

          img {
            width: 160px;
          }
        }
    }
  }

  @media (max-width: 576px) {
    .prizes_block {
      &_first_line {
        margin-top: 10px;
        
        img {
          width: 30%;
        }
      }

      &_second_line {
        width: 80%;
      }
    }
  }
</style>