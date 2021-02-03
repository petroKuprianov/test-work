<template>
  <div>
    <header-nav></header-nav>
    <article-chart></article-chart>
    <main-page></main-page>
    <contact></contact>
    <footer-nav></footer-nav>
  </div>
</template>

<script>

import headerNav from "@/components/header-nav";
import articleChart from '@/components/article-chart';
import mainPage from '@/components/main-page';
import contact from "@/components/contact";
import footerNav from "@/components/footer-nav";

export default {
  name: 'App',
  components: {
    headerNav,
    articleChart,
    mainPage,
    contact,
    footerNav
  }
}
</script>

<style>
@font-face {
  font-family: 'MuseoSansCyrl-500';
  src: url('./fonts/museosanscyrl-500.eot');
  src: url('./fonts/museosanscyrl-500.eot?#iefix') format('embedded-opentype'),
  url('./fonts/museosanscyrl-500.woff2') format('woff2'),
  url('./fonts/museosanscyrl-500.woff') format('woff'),
  url('./fonts/museosanscyrl-500.ttf') format('truetype'),
  url('./fonts/museosanscyrl-500.svg#museosanscyrl-500') format('svg');
}
@font-face {
  font-family: 'Montserrat';
  src: url('./fonts/Montserrat-Regular.ttf');
}
body{
  margin: 0;
  padding: 0;
}
p{
  font-family: MuseoSansCyrl-500, SansSerif;
  margin: 0;
  padding: 0;
}
ul{
  padding: 0;
  margin: 0;
}
li{
  margin: 0;
  padding: 0;
}
a{
  text-decoration: none;
}
</style>
