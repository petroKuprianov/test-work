<template>
<header class="header">
  <a href="" class="header__logo">
    <p class="header__logo-text">LOGO</p>
  </a>
  <nav class="header__nav">
    <ul class="header__nav-list">
      <li class="header__nav-item">
        <p>How it works</p>
      </li>
      <li class="header__nav-item">
        <p>About</p>
      </li>
      <li class="header__nav-item">
        <p>Instructions</p>
      </li>
      <li class="header__nav-item">
        <p>Accounts</p>
      </li>
      <li class="header__nav-item">
        <p>Platforms</p>
      </li>
      <li class="header__nav-item">
        <p>Contact</p>
      </li>
    </ul>
  </nav>
  <div class="header__sign">
    <button id="button_sign">
      <p>Sign in for free</p>
    </button>
  </div>
  <div class="header__select">
    <p>EN</p>
    <img src="../assets/Vector.svg" alt="Vector">
  </div>

</header>
</template>

<script>
export default {
name: "header-nav",
}
</script>

<style scoped lang="scss">
.header{
  width: 100%;
  height: 80px;
  background-color: #FFFFFF;
  &__logo{
    float: left;
    margin-top: 32px;
    margin-left: 120px;
    &-text{
      font-style: normal;
      font-weight: bold;
      font-size: 15px;
      line-height: 16px;
      color: #333333;
    }
  }
  &__nav{
    float: left;
    margin-left: 57px;
    margin-top: 32px;
    &-list{
      display: flex;
      list-style: none;
      padding: 0;
      margin: 0;
    }
    &-item{
      margin-left: 32px;
    }
    &-item:first-child{
      margin-left: 0;
    }
  }
  &__select{
    float: right;
    width: 80px;
    height: 40px;
    border: 1px solid #000000;
    box-sizing: border-box;
    border-radius: 60px;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    margin-top: 20px;
    margin-right: 24px;
    p{
      font-style: normal;
      font-weight: 500;
      font-size: 15px;
      line-height: 16px;
      color: #333333;
    }
    img{
      width: 9px;
      height: 5px;
    }
  }
  &__sign{
    button {
      float: right;
      padding: 13px 24px;
      width: 167px;
      height: 40px;
      background: #6248FF;
      border-radius: 60px;
      border: none;
      margin-top: 20px;
      margin-right: 60px;
      transition: 0.5s;
      outline: none;
      p{
        font-style: normal;
        font-weight: 500;
        font-size: 14px;
        line-height: 14px;
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
</style>
