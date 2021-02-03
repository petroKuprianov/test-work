<template>
<footer class="footer">
  <div class="footer__top">
    <a href="" class="footer__logo">
      <p class="footer__logo-text">LOGO</p>
    </a>
    <div class="footer__top-warning">
      <p class="footer__top-warning-header">Information and high risk warning: </p>
      <div class="footer__top-warning-wrapper">
        <p class="footer__top-warning-wrapper-text">
          Trading with foreign exchange (FX), contract for differences (CFDs) and
          precious metals carries a high level of risk that may not be suitable for
          all investors. Leverage creates additional risk and loss exposure.
          Before you decide to trade foreign exchange or contract for differences,
          carefully consider your investment objectives, experience level, and risk tolerance.
        </p>
      </div>
    </div>
    <div class="footer__top-disclaimer">
      <p class="footer__top-disclaimer-header">Legal disclaimer:</p>
      <div class="footer__top-disclaimer-wrapper">
        <p class="footer__top-disclaimer-wrapper-text">
          Forex trading entails significant risks and is not appropriate
          for all investors. The possibility of incurring substantial
          losses should be taken into account. It is therefore important to
          understand the possible consequences of investing. Traders should
          weigh their earning potential against the risks involved and
          act accordingly. Interactive Trade Ltd operating under brand
          and using domenLink domain within the European Economic Area.
        </p>
      </div>
    </div>
    <div class="footer__top-nav">
      <ul class="footer__top-nav-list">
        <li class="footer__top-nav-list-item"><a href="#">
          <p>About us</p>
        </a></li>
        <li class="footer__top-nav-list-item"><a href="#">
          <p>Instructions</p>
        </a></li>
        <li class="footer__top-nav-list-item"><a href="#">
          <p>Platforms</p>
        </a></li>
        <li class="footer__top-nav-list-item"><a href="#">
          <p>Contact Us</p>
        </a></li>
        <li class="footer__top-nav-list-item"><a href="#">
          <p>Sign in</p>
        </a></li>
        <li class="footer__top-nav-list-item"><a href="#">
          <p>Sign up for free</p>
        </a></li>
      </ul>
    </div>
  </div>
  <div class="footer__bottom">
    <div class="footer__bottom-wrapper">
      <p class="footer__bottom-wrapper-copyright">Copyright 2020, All Right Reserved</p>
      <a class="footer__bottom-wrapper-terms" href="">
        <p class="footer__bottom-wrapper-terms">Terms and Conditions</p>
      </a>
      <a href="">
        <p class="footer__bottom-wrapper-privacy">Privacy Policy</p>
      </a>
      <a href="">
        <p class="footer__bottom-wrapper-risk">Risk Warnings</p>
      </a>
      <a href="">
        <p class="footer__bottom-wrapper-laundering">Anti-Money Laundering</p>
      </a>
    </div>
  </div>
</footer>
</template>

<script>
export default {
  name: "footer-nav"
}
</script>

<style scoped lang="scss">
.footer{
  width: 100%;
  //padding: 32px 120px;
  &__logo{
    &-text{
      font-style: normal;
      font-weight: bold;
      font-size: 15px;
      line-height: 16px;
      color: #000000;
    }
  }
  &__top{
    display: flex;
    align-items: flex-start;
    justify-content: space-evenly;
    margin-top: 32px;
    margin-left: 120px;
    &-warning{
      margin-left: 160px;
      &-header{
        font-style: normal;
        font-weight: 500;
        font-size: 18px;
        line-height: 30px;
        color: #333333;
      }
      &-wrapper{
        width: 380px;
        margin-top: 16px;
        &-text{
          font-family: Montserrat;
          font-style: normal;
          font-weight: normal;
          font-size: 16px;
          line-height: 27px;
          color: #4F4F4F;
        }
      }

    }
    &-disclaimer{
      margin-left: 30px;
      &-header{
        font-style: normal;
        font-weight: 500;
        font-size: 18px;
        line-height: 30px;
        color: #333333;
      }
      &-wrapper{
        width: 380px;
        margin-top: 16px;
        &-text{
          font-family: Montserrat;
          font-style: normal;
          font-weight: normal;
          font-size: 16px;
          line-height: 27px;
          color: #4F4F4F;
        }
      }
    }
    &-nav{
      margin-left: 96px;
      &-list{
        list-style: none;
        padding: 0;
        margin: 0;
        &-item{
          a{
            p{
              font-style: normal;
              font-weight: 500;
              font-size: 15px;
              line-height: 16px;
              color: #333333;
            }
          }
        }
        &-item:not(:first-child){
          margin-top: 24px;
        }
      }
    }
  }
  &__bottom{
    margin-top: 48px;
    margin-left: 120px;
    margin-bottom: 72px;
    &-wrapper{
      display: flex;
      justify-content: space-evenly;
      &-copyright{
        font-family: Montserrat;
        font-style: normal;
        font-weight: normal;
        font-size: 16px;
        line-height: 27px;
        color: #828282;
      }
      a{
        p{
          font-family: Montserrat;
          font-style: normal;
          font-weight: normal;
          font-size: 16px;
          line-height: 27px;
          color: #828282;
          margin-left: 66px;
        }
      }
     &-terms{
        margin-left: 66px;
      }
    }
  }
}
</style>
