<template>
<div class="chart">
  <div class="chart__overlay"></div>
  <div class="chart__info">
    <div class="chart__info-header">
      <p>Trade everywhere. Invest here!</p>
    </div>
    <div class="chart__info-main">
      <p>
        We provide only the best trading software.
        The trading terminal MetaTrader4 is the most
        popular and convenient platform for access to global exchanges.
        You can work anywhere.
      </p>
    </div>
    <div class="chart__info-btn">
      <button id="button_start">
        <p>Start trading</p>
      </button>
    </div>
  </div>
  <div class="chart__img">
    <img src="../assets/chart.svg" alt="Chart img">
  </div>
</div>
</template>

<script>
export default {
  name: "article-chart",

}
</script>

<style scoped lang="scss">
.chart{
  width: 100%;
  height: 720px;
  display: flex;
  justify-content: space-between;
  &__overlay{
    position: absolute;
    width: 100%;
    height: inherit;
    background: #6248FF;
    opacity: 0.1;
    z-index: -1;
  }
  &__info{
    display: flex;
    float: left;
    flex-direction: column;
    margin-top: 140px;
    margin-left: 120px;
    &-header{
      max-width: 585px;
      max-height: 144px;
      p{
        font-style: normal;
        font-weight: 500;
        font-size: 64px;
        line-height: 72px;
        color: #333333;
      }
    }
    &-main{
      width: 483px;
      height: 120px;
      margin-top: 32px;
      p{
        font-family: Montserrat;
        font-style: normal;
        font-weight: normal;
        font-size: 18px;
        line-height: 30px;
        color: #4F4F4F;
      }
    }
    &-btn{

      button{
        margin-top: 48px;
        width: 257px;
        height: 54px;
        background-color: #6248FF;
        border-radius: 60px;
        border: none;
        transition: 1s;
        outline: none;
        p{
          font-style: normal;
          font-weight: 500;
          font-size: 16px;
          line-height: 14px;
          text-align: center;
          letter-spacing: 0.03em;
          text-transform: uppercase;
          color: #FFFFFF;
        }
      }
      button:hover{
        background: #7181FC;
        cursor: pointer;
      }
      button:active{
        background: #354BF4;
      }
    }
  }
  &__img{
    margin-top: 100px;
    margin-right: 120px;
    img{
      width: 482px;
      height: 519px;
    }
  }
}
</style>
