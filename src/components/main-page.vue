<template>
<main class="main">

  <div class="main__steps">
    <div class="main__header">
      <div class="main__overlay"></div>
    <span>
      Getting Started Is
    </span>

      <span>Fast & Easy</span>
    </div>
    <div class="main__steps-container">
    <div class="main__steps-left">
      <div class="main__steps-left-step">
        <p class="main__steps-left-step-number">01.</p>
        <p class="main__steps-left-step-header">Register</p>
        <p class="main__steps-left-step-info">Complete the simple registration to get your trading credentials.</p>
      </div>
      <div class="main__vector">
        <img src="../assets/Vector2.svg" alt="Vector img">
      </div>
      <div class="main__steps-left-step main__steps-left-second">
        <p class="main__steps-left-step-number">03.</p>
        <p class="main__steps-left-step-header">Register</p>
        <p class="main__steps-left-step-info">Complete the simple registration to get your trading credentials.</p>
      </div>
      <div class="main__vector2">
        <img src="../assets/Vector2.svg" alt="Vector img">
      </div>
    </div>
    <div class="main__steps-right">
      <div class="main__steps-right-step">
        <p class="main__steps-right-step-number">02.</p>
        <p class="main__steps-right-step-header">Register</p>
        <p class="main__steps-right-step-info">Complete the simple registration to get your trading credentials.</p>
      </div>
          <div class="main__vector3">
            <img src="../assets/Vector3.svg" alt="Vector img">
          </div>
      <div class="main__steps-right-step">
        <p class="main__steps-right-step-number">04.</p>
        <p class="main__steps-right-step-header">Register</p>
        <p class="main__steps-right-step-info">Complete the simple registration to get your trading credentials.</p>
      </div>
    </div>
    </div>

    <div class="main__steps-containerMob">
      <div class="main__steps-containerMob-step">
        <p class="main__steps-containerMob-step-number">01.</p>
        <p class="main__steps-containerMob-step-header">Register</p>
        <p class="main__steps-containerMob-step-info">Complete the simple registration to get your trading credentials.</p>
      </div>
      <div class="main__steps-containerMob-step">
        <p class="main__steps-containerMob-step-number">02.</p>
        <p class="main__steps-containerMob-step-header">Register</p>
        <p class="main__steps-containerMob-step-info">Complete the simple registration to get your trading credentials.</p>
      </div>
      <div class="main__steps-containerMob-step">
        <p class="main__steps-containerMob-step-number">03.</p>
        <p class="main__steps-containerMob-step-header">Register</p>
        <p class="main__steps-containerMob-step-info">Complete the simple registration to get your trading credentials.</p>
      </div>
      <div class="main__steps-containerMob-step">
        <p class="main__steps-containerMob-step-number">04.</p>
        <p class="main__steps-containerMob-step-header">Register</p>
        <p class="main__steps-containerMob-step-info">Complete the simple registration to get your trading credentials.</p>
      </div>
    </div>

  </div>
  <div class="main__invest">
    <div class="main__invest-left">
      <div class="main__invest-left-info">
        <div class="main__overlay"></div>
        <span>
          People love Big
        </span>
        <span>Invest</span>
      </div>
      <div class="main__invest-left-swiper">
        <button class="main__invest-left-btn main__invest-left-swiper-first" @click="showPrev" :disabled="isCurrent === 1">
          <img src="../assets/Vector.svg" alt="Vector img">
        </button>
        <button class="main__invest-left-btn main__invest-left-swiper-second" @click="showNext" :disabled="isCurrent === 3">
          <img src="../assets/Vector.svg" alt="Vector img">
        </button>
      </div>
    </div>
    <img class="main__invest-scope" src="../assets/scope.svg" alt="Scope img">
  <transition name="fade" :duration="{ enter: 300, leave: 400 }" mode="out-in">
    <div key="first" v-if="isCurrent === 1" class="main__invest-right">
      <div class="main__invest-right-name">
        <div class="main__invest-right-name-photo">
          <img src="../assets/Photo.png" alt="Photo icon">
        </div>
        <div class="main__invest-right-name-text">
          <p>Albert Abello</p>
          <p>Director of Growth</p>
        </div>
        <img class="main__invest-scopeMob" src="../assets/scope.svg" alt="Scope img">
      </div>
      <div class="main__invest-right-comment">
        <p>This magical product actually works! It has radically
          changed the way we build our audiences. Increasing new
          customer sales by 6x in our most mature market.
        </p>
      </div>
      <div class="main__invest-right-mark">
        <p>01 / 04</p>
      </div>
    </div>

    <div key="second" v-if="isCurrent === 2" class="main__invest-right">
      <div class="main__invest-right-name">
        <div class="main__invest-right-name-photo">
          <img src="../assets/Photo.png" alt="Photo icon">
        </div>
        <div class="main__invest-right-name-text">
          <p>Albert Abello</p>
          <p>Director of Growth</p>
        </div>
        <img class="main__invest-scopeMob" src="../assets/scope.svg" alt="Scope img">
      </div>
      <div class="main__invest-right-comment">
        <p>This magical product actually works! It has radically
          changed the way we build our audiences. Increasing new
          customer sales by 6x in our most mature market.
        </p>
      </div>
      <div class="main__invest-right-mark">
        <p>01 / 05</p>
      </div>
    </div>

    <div key="third" v-if="isCurrent === 3" class="main__invest-right">
      <div class="main__invest-right-name">
        <div class="main__invest-right-name-photo">
          <img src="../assets/Photo.png" alt="Photo icon">
        </div>
        <div class="main__invest-right-name-text">
          <p>Albert Abello</p>
          <p>Director of Growth</p>
        </div>
        <img class="main__invest-scopeMob" src="../assets/scope.svg" alt="Scope img">
      </div>
      <div class="main__invest-right-comment">
        <p>This magical product actually works! It has radically
          changed the way we build our audiences. Increasing new
          customer sales by 6x in our most mature market.
        </p>
      </div>
      <div class="main__invest-right-mark">
        <p>01 / 06</p>
      </div>
    </div>
  </transition>

  </div>
  <div class="main__questions">
    <div class="main__questions-info">
        <span>
          Frequently asked
        </span>
      <div class="main__overlay"></div>
      <span>questions</span>
    </div>
    <div class="main__questions-items">
      <div class="main__questions-items-item" @click="show(0)">
        <div>
          <p class="main__questions-items-item-header">How do I change my details?</p>
          <img @click="show(0)" src="../assets/bi_plus.svg" alt="icon plus" :class="isVisible[0] === true ? 'rotate' : ''">
        </div>
        <div v-if="isVisible[0]" class="main__questions-items-item-more">
          <p>
            We provide only the best trading software.
            The trading terminal MetaTrader4 is the most popular
            and convenient platform for access to global exchanges.
            You can work anywhere. All you need is the Internet because
            the necessary trading tools are already collected in one place
            and are available in a couple of clicks. Use only the best and
            develop with us!
          </p>
        </div>
      </div>

      <div class="main__questions-items-item" @click="show(1)">
        <div>
          <p class="main__questions-items-item-header">How do I change my details?</p>
          <img src="../assets/bi_plus.svg" alt="icon plus" :class="isVisible[1] === true ? 'rotate' : ''">
        </div>
        <div v-if="isVisible[1]" class="main__questions-items-item-more">
          <p>
            We provide only the best trading software.
            The trading terminal MetaTrader4 is the most popular
            and convenient platform for access to global exchanges.
            You can work anywhere. All you need is the Internet because
            the necessary trading tools are already collected in one place
            and are available in a couple of clicks. Use only the best and
            develop with us!
          </p>
        </div>
      </div>

      <div class="main__questions-items-item" @click="show(2)">
        <div>
          <p class="main__questions-items-item-header">How do I change my details?</p>
          <img src="../assets/bi_plus.svg" alt="icon plus" :class="isVisible[2] === true ? 'rotate' : ''">
        </div>
        <div v-if="isVisible[2]" class="main__questions-items-item-more">
          <p>
            We provide only the best trading software.
            The trading terminal MetaTrader4 is the most popular
            and convenient platform for access to global exchanges.
            You can work anywhere. All you need is the Internet because
            the necessary trading tools are already collected in one place
            and are available in a couple of clicks. Use only the best and
            develop with us!
          </p>
        </div>
      </div>

      <div class="main__questions-items-item" @click="show(3)">
        <div>
          <p class="main__questions-items-item-header">How do I change my details?</p>
          <img src="../assets/bi_plus.svg" alt="icon plus" :class="isVisible[3] === true ? 'rotate' : ''">
        </div>
        <div v-if="isVisible[3]" class="main__questions-items-item-more">
          <p>
            We provide only the best trading software.
            The trading terminal MetaTrader4 is the most popular
            and convenient platform for access to global exchanges.
            You can work anywhere. All you need is the Internet because
            the necessary trading tools are already collected in one place
            and are available in a couple of clicks. Use only the best and
            develop with us!
          </p>
        </div>
      </div>

      <div class="main__questions-items-item" @click="show(4)">
        <div>
          <p class="main__questions-items-item-header">How do I change my details?</p>
          <img src="../assets/bi_plus.svg" alt="icon plus" :class="isVisible[4] === true ? 'rotate' : ''">
        </div>
        <div v-if="isVisible[4]" class="main__questions-items-item-more">
          <p>
            We provide only the best trading software.
            The trading terminal MetaTrader4 is the most popular
            and convenient platform for access to global exchanges.
            You can work anywhere. All you need is the Internet because
            the necessary trading tools are already collected in one place
            and are available in a couple of clicks. Use only the best and
            develop with us!
          </p>
        </div>
      </div>

      <div class="main__questions-items-item" @click="show(5)">
        <div>
          <p class="main__questions-items-item-header">How do I change my details?</p>
          <img src="../assets/bi_plus.svg" alt="icon plus" :class="isVisible[5] === true ? 'rotate' : ''">
        </div>
        <div v-if="isVisible[5]" class="main__questions-items-item-more">
          <p>
            We provide only the best trading software.
            The trading terminal MetaTrader4 is the most popular
            and convenient platform for access to global exchanges.
            You can work anywhere. All you need is the Internet because
            the necessary trading tools are already collected in one place
            and are available in a couple of clicks. Use only the best and
            develop with us!
          </p>
        </div>
      </div>

      <div class="main__questions-items-item" @click="show(6)">
        <div>
          <p class="main__questions-items-item-header">How do I change my details?</p>
          <img src="../assets/bi_plus.svg" alt="icon plus" :class="isVisible[6] === true ? 'rotate' : ''">
        </div>
        <div v-if="isVisible[6]" class="main__questions-items-item-more">
          <p>
            We provide only the best trading software.
            The trading terminal MetaTrader4 is the most popular
            and convenient platform for access to global exchanges.
            You can work anywhere. All you need is the Internet because
            the necessary trading tools are already collected in one place
            and are available in a couple of clicks. Use only the best and
            develop with us!
          </p>
        </div>
      </div>

    </div>

  </div>
</main>
</template>

<script>
export default {
  name: "main-page",
  data(){
    return{
      isCurrent: 1,
      isVisible: {
        0:false,
        1:false,
        2:false,
        3:false,
        4:false,
        5:false,
        6:false
      }
      }
  },
  methods: {
    showPrev() {
      this.isCurrent -= 1;
    },
    showNext() {
      this.isCurrent += 1;
    },
    show(item){
      if(this.isVisible[item] === true)
      {
        this.isVisible[item] = false;
      }
      else{
        for(let i in this.isVisible) {
          this.isVisible[i] = false;
        }
        this.isVisible[item] = true;
      }

    }
  }
}
</script>

<style scoped lang="scss">
.main{
  padding: 140px 120px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-start;
  &__header{
    max-width: 483px;
    span{
      font-family: MuseoSansCyrl-500;
      font-style: normal;
      font-weight: 600;
      font-size: 56px;
      line-height: 66px;
      color: #333333;
    }
  }
  &__overlay{
    position: absolute;
    width: 300px;
    height: 72px;
    background: #6248FF;
    opacity: 0.1;
  }
  &__steps{
    margin-top: 60px;
    display: flex;
    &-container{
      display: flex;
    }
    &-containerMob{
      display: none;
    }
    &-left {
      display: flex;
      flex-direction: column;
      &-step {
        float: left;
        width: 483px;
        height: 203px;
        padding: 32px;
        background: #FFFFFF;
        border: 2px solid #6248FF;
        box-sizing: border-box;
        border-radius: 30px;

        &-number {
          font-style: normal;
          font-weight: 500;
          font-size: 15px;
          line-height: 18px;
          color: #6248FF;
        }

        &-header {
          margin-top: 8px;
          font-style: normal;
          font-weight: 500;
          font-size: 24px;
          line-height: 29px;
          color: #333333;
        }

        &-info {
          font-family: Montserrat;
          margin-top: 24px;
          font-style: normal;
          font-weight: normal;
          font-size: 18px;
          line-height: 30px;
          color: #4F4F4F;
        }

        &-second {
          margin-left: 132px;
        }
      }
      &-second{
        margin-top: 130px;
      }
    }
    &-right{
      display: flex;
      flex-direction: column;
      margin-top: 164px;
      margin-left: 132px;
      &-step {
        width: 483px;
        height: 203px;
        padding: 32px;
        background: #FFFFFF;
        border: 2px solid #6248FF;
        box-sizing: border-box;
        border-radius: 30px;

        &-number {
          font-style: normal;
          font-weight: 500;
          font-size: 15px;
          line-height: 18px;
          color: #6248FF;
        }

        &-header {
          margin-top: 8px;
          font-style: normal;
          font-weight: 500;
          font-size: 24px;
          line-height: 29px;
          color: #333333;
        }

        &-info {
          font-family: Montserrat;
          margin-top: 24px;
          font-style: normal;
          font-weight: normal;
          font-size: 18px;
          line-height: 30px;
          color: #4F4F4F;
        }

        &-second {
          margin-left: 132px;
        }
      }
      &-step:last-child{
        margin-top: 130px;
      }
    }
  }
  &__vector{
    margin-top: 87px;
    position: absolute;
    float: left;
    left: 1085px;
    img{
      max-width: 374px;
    }
  }
  &__vector2{
    margin-top: 423px;
    position: absolute;
    left: 1085px;
  }
  &__vector3{
    margin-top: 93px;
    position: absolute;
    left: 840px;
  }
  &__invest{
    display: flex;
    &-left{
      margin-top: 140px;
      &-info{
        max-width: 483px;
        span{
          font-family: MuseoSansCyrl-500;
          font-style: normal;
          font-weight: 600;
          font-size: 56px;
          line-height: 66px;
          color: #333333;
        }
      }
      &-swiper{
        display: flex;
        margin-top: 40px;
        &-second{
          margin-left: 16px;
          img{
            transform: rotate(-90deg) !important;
          }
        }
      }
      &-btn{
        width: 48px;
        height: 48px;
        border: 1px solid #E0E0E0;
        border-radius: 100%;
        box-sizing: border-box;
        display: flex;
        justify-content: center;
        align-items: center;
        outline: none;
        img{
          transform: rotate(90deg);
        }
      }
      &-btn:hover{
        border: 1px solid #6248FF;
      }

    }
    &-scope{
      margin-left: 132px;
      margin-top: 97px;
      margin-right: 15px;
    }
    &-scopeMob{
      display: none;
    }
    &-right{
      margin-top: 167px;
      height: 380px;
      &-name{
        display: flex;
        &-text{
          margin-left: 30px;
        }
        &-text p{
          font-style: normal;
          font-weight: 500;
          font-size: 18px;
          line-height: 30px;
          color: #333333;
        }
        &-text p:last-child{
          margin-top: 8px;
          font-family: Montserrat;
          font-style: normal;
          font-weight: normal;
          font-size: 16px;
          line-height: 27px;
          color: #4F4F4F;
        }
      }
      &-comment{
        width: 585px;
        margin-top: 17px;
        p{
          font-style: normal;
          font-weight: 500;
          font-size: 24px;
          line-height: 29px;
          color: #333333;
        }
      }
      &-mark{
        margin-top: 30px;
        p{
          font-style: normal;
          font-weight: 500;
          font-size: 15px;
          line-height: 18px;
          color: #6248FF;
        }
      }
    }
  }
  &__questions{
    margin-top: 140px;
    display:flex;
    justify-content: space-evenly;
    &-info{
      max-width: 483px;
      span{
        font-family: MuseoSansCyrl-500;
        font-style: normal;
        font-weight: 600;
        font-size: 56px;
        line-height: 66px;
        color: #333333;
      }
    }
    &-items{
      margin-left: 100px;
      margin-top: 68px;
      &-item{
        width: 995px;
        //height: 96px;
        background: #FFFFFF;
        border: 2px solid #6248FF;
        box-sizing: border-box;
        border-radius: 20px;
        padding: 34px 40px;
        display: flex;
        flex-direction: column;
        &-header{
          font-style: normal;
          font-weight: 500;
          font-size: 24px;
          line-height: 29px;
          color: #333333;
        }
        &-more{
          font-family: Montserrat;
          font-style: normal;
          font-weight: normal;
          font-size: 16px;
          line-height: 27px;
          color: #4F4F4F;
          max-width: 750px;
          margin-top: 24px;
        }
        div {
          display: flex;
          justify-content: space-between;
        }

      }
      &-item:not(:first-child){
        margin-top: 16px;
      }

    }
  }
  &__overlay{
    position: absolute;
    width: 300px;
    height: 72px;
    background: #6248FF;
    opacity: 0.1;
  }
}
.fade-enter-active, .fade-leave-active {
  transition: opacity .3s;
}
.fade-enter, .fade-leave-active /* .fade-leave-active до версии 2.1.8 */ {
  opacity: 0;
}
.rotate{
  transform: rotate(45deg);
}


@media screen and (max-width: 1820px){
.main{
  display: block;
  padding-right: 60px;
  &__steps{
    flex-direction: column;
    &-container{
      display: flex;
    }
    &-left{
      margin-top: 70px;
    }
    &-right{
      margin-top: 230px;
    }
  }
  &__questions{
    display: block;
  }
  &__vector{
    margin-top: 87px;
    position: absolute;
    float: left;
    left: 602px;
    img{
      max-width: 374px;
    }
  }
  &__vector2{
    margin-top: 423px;
    position: absolute;
    left: 602px;
  }
  &__vector3{
    position: absolute;
    left: 358px;
  }
  &__questions{
    &-items{
      &-item{
        width: 100%;
      }
    }
  }
}
}

@media screen and (max-width: 1250px){
  .main{
    padding-left: 60px;
    padding-right: 60px;
    &__steps{
      &-left{
        &-step{
          width: 329px;
          height: 233px;

        }
        &-second{
          margin-top: 85px;
        }
      }
      &-right{
        margin-top: 210px;
        margin-left: 60px;
        &-step{
          width: 329px;
          height: 233px;
        }
        &-step:last-child{
          margin-top: 110px;
        }
      }
    }


    &__vector{
      margin-top: 90px;
      position: absolute;
      float: left;
      left: 390px;
      img{
        max-width: 250px;
      }
    }
    &__vector2{
      margin-top: 433px;
      position: absolute;
      left: 390px;
      img{
        width: 250px;
      }
    }
    &__vector3{
      margin-top: 130px;
      position: absolute;
      left: 200px;
      img{
        max-width: 250px;
      }
    }
    &__invest{
      &-scope{
        margin-left: 62px;
      }
      &-left{
        &-info{
          max-width: 483px;
          span{
            //font-size: 46px;
          }
        }
      }
      &-right{
        &-comment{
          width: 400px;
        }
      }
    }

      &__questions{
        &-items{
          margin-left: 0;
          &-item{
            width: 100%;
          }
        }
      }
    }

}

@media screen and (max-width: 800px) {
  .main{
    padding-top: 120px;
    &__steps{
      margin-top: 0;
      &-right{
        margin-left: 30px;
      }
    }
    &__vector3{
      margin-top: 130px;
      position: absolute;
      left: 225px;
      img{
        width: 193px;
        height: 58px;
      }
    }
    &__vector{
      margin-top: 95px;
      position: absolute;
      float: left;
      left: 390px;
      img{
        width: 193px;
        height: 58px;
      }
    }
    &__vector2{
      margin-top: 433px;
      position: absolute;
      left: 390px;
      img{
        width: 193px;
        height: 58px;
      }
    }
    &__invest{
      flex-direction: column;
      &-scope{
        //width: 33px;
        //position: absolute;
        //margin-top: 455px;
        //left: 350px;
        display: none;
      }
      &-scopeMob{
        display: block;
        margin-top: 16px;
      }
      &-left{
        &-swiper{
          &-first{
            position: absolute;
            margin-top: 140px;
          }
          &-second{
            position: absolute;
            margin-top: 140px;
            left: 640px;
          }
        }
      }

      &-right{
        display: flex;
        flex-direction: column;
        align-items: center;
        margin-top: 0;
        &-name{
          flex-direction: column;
          align-items: center;
          text-align: center;
        }
        &-comment{
          width: 508px;
          text-align: center;
          margin-top: 30px;
          text-align: center;
        }
      }
    }
  }

}
@media screen and (max-width: 758px){
  .main{
    padding-left: 20px;
    &__header{
      span{
        font-size: 40px;
        line-height: 44px;
      }
    }
    &__steps{
      &-container{
        display: none;
      }
      &-containerMob{
        display: block;
        display: flex;
        flex-direction: column;
        &-step{
          width: 280px;
          height: 217px;
          background: #FFFFFF;
          border: 2px solid #4F62F6;
          box-sizing: border-box;
          border-radius: 30px;
          &-number{
              font-style: normal;
              font-weight: 500;
              font-size: 15px;
              line-height: 18px;
              color: #4F62F6;
          }
        }
      }
    }
  }
}

</style>
<!--<div class="main__steps-containerMob-step">-->
<!--<p class="main__steps-containerMob-step-number">04.</p>-->
<!--<p class="main__steps-containerMob-step-header">Register</p>-->
<!--<p class="main__steps-containerMob-step-info">Complete the simple registration to get your trading credentials.</p>-->
<!--</div>-->
