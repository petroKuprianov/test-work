<template>
<div class="contact">
  <div class="contact__overlay"></div>
  <div class="contact__wrapper">
    <div class="contact__wrapper-info">
      <p class="contact__wrapper-info-header">Contact us!</p>
      <div class="contact__wrapper-info-main">
        <p>The support staff and customer service are available to help you with any questions or needs you might have. Just drop us a line.</p>
      </div>
      <p class="contact__wrapper-info-owner">This site is owned and operated by Kode Tech Solutions LTD</p>
      <p class="contact__wrapper-info-address contact__wrapper-info-addressFirst">Phone:</p>
      <p class="contact__wrapper-info-addressValue">442038857261</p>
      <p class="contact__wrapper-info-address">Email:</p>
      <p class="contact__wrapper-info-addressValue">help@google.com</p>
      <p class="contact__wrapper-info-address">Address:</p>
      <div class="contact__wrapper-info-addressWrap">
        <p class="contact__wrapper-info-addressValue">Trust Company Complex, Ajeltake Road, Ajeltake Island, Majuro, Republic of the Marshall Islands, MH 96960</p>
      </div>
    </div>
    <form class="contact__wrapper-form" action="#">
        <input type="text" class="contact__wrapper-form-name" placeholder="Name">
        <input type="text" class="contact__wrapper-form-email" placeholder="Email"  v-model="inputEmail" @input="validateEmail" :class="isCorrectEmail && inputEmail.length ? 'contact__wrapper-form-correct': ''">
        <p class="contact__wrapper-form-check" v-if="!isCorrectEmail && inputEmail.length">Incorrect email type</p>
        <input type="text" class="contact__wrapper-form-msg" placeholder="Message">
        <input class="contact__wrapper-form-submit" type="submit" value="send" :disabled="!isCorrectEmail">
    </form>
  </div>
</div>
</template>

<script>
export default {
  name: "contact",
  data(){
    return{
      inputEmail: '',
      isCorrectEmail: false,
    }
  },
  methods:{
    validateEmail() {
      const re = /^(([^<>()[\]\\.,;:\s@"]+(\.[^<>()[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/;
      this.isCorrectEmail = re.test(String(this.inputEmail).toLowerCase());
  },
  }
}
</script>

<style scoped lang="scss">
.contact{
  width: 100%;
  min-height: 739px;
  &__overlay{
    width: 100%;
    min-height: 739px;
    position:absolute;
    background: #6248FF;
    opacity: 0.08;
    z-index: -1;
  }
  &__wrapper{
    padding: 120px;
    display: flex;
    justify-content: space-between;
    &-info{
      &-header{
        font-style: normal;
        font-weight: 500;
        font-size: 56px;
        line-height: 66px;
        color: #333333;
      }
      &-main{
        width: 483px;
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
      &-owner{
        font-family: Montserrat;
        font-style: normal;
        font-weight: normal;
        font-size: 16px;
        line-height: 27px;
        color: #4F4F4F;
        margin-top: 48px;
      }
      &-address{
        font-style: normal;
        font-weight: 500;
        font-size: 15px;
        line-height: 16px;
        color: #333333;
        margin-top: 16px;
      }
      &-addressFirst{
        margin-top: 24px;
      }
      &-addressValue{
        font-family: Montserrat;
        font-style: normal;
        font-weight: normal;
        font-size: 16px;
        line-height: 27px;
        color: #4F4F4F;
        margin-top: 8px;
    }
      &-addressWrap{
        width: 483px;
      }

    }
    &-form{
        width: 585px;
        padding: 80px;
        background: #FFFFFF;
        border: 2px solid #6248FF;
        box-sizing: border-box;
        border-radius: 20px;
        display: flex;
        flex-direction: column;
        margin-top: 14px;
        &-name, &-email, &-msg{
          width: 425px;
          height: 40px;
          border: 1px solid #E0E0E0;
          box-sizing: border-box;
          border-radius: 3px;
          padding: 7px 16px;
          font-family: Montserrat;
          font-style: normal;
          font-weight: normal;
          font-size: 16px;
          line-height: 26px;
          color: #828282;
        }
      &-name:focus,&-email:focus, &-msg:focus{
        outline: none;
        border: 1px solid #828282;
        color: #4F4F4F;
      }
      &-check{
        font-style: normal;
        font-weight: 500;
        font-size: 15px;
        line-height: 16px;
        color: #EB5757;
        margin-top: 8px;
      }
      &-correct{
        border: 1px solid #0EAC00;
      }
        input:not(:first-child){
          margin-top: 24px;
        }
        input:last-child{
          width: 172px;
          height: 54px;
          background: #6248FF;
          border-radius: 60px;
          align-self: center;
          margin-top: 40px;
          font-style: normal;
          font-weight: 500;
          font-size: 16px;
          line-height: 14px;
          text-align: center;
          letter-spacing: 0.03em;
          text-transform: uppercase;
          color: #FFFFFF;
          border: none;
          outline: none;
        }
      }

    }
}

</style>
