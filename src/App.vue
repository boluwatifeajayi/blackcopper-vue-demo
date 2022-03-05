"/eslint-disable no-trailing-spaces/"
<template>
<div class="container">
<VueHeader/>
<TotalInvestment/>
<CurrentInvestment/>
</div>
</template>
<script>
import VueHeader from './components/VueHeader'
// import VueBody from './components/VueBody';
import TotalInvestment from './components/TotalInvestment'
import CurrentInvestment from './components/CurrentInvestment'
export default {
  name: 'App',
  components: {
    VueHeader,
    TotalInvestment,
    CurrentInvestment
  }
}
</script>
<style>
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
:root {
    --primary-color: rgb(245, 195, 57);
    --secondary-color: #333;
    --overlay-color: rgba(0, 0, 0, 0.7);
}
body {
  font-family: 'Montserrat', sans-serif;
  line-height: 1.6;
  color: #333;
  background-color:#f0f6fc;
}
html{
    scroll-behavior: smooth;
    overflow-x: hidden;
}
a{
    text-decoration: none;
}
ul {
    list-style: none;
}

/*NAV BAR*/

header {
    height: 15vh;
    width: 100%;

}
.logo {

    float: left;
    margin: 16px 75px;
    color: #fff;
    font-weight: bold;
    font-size: 21px;
}
.logo a{
    text-decoration: none;
    color: #333;
}

nav {
    position: fixed;
    width: 100%;
    z-index: 3000;
    background-color: white;
}
nav ul {
    list-style: none;
    background: rgba(0, 0, 0, 0);
    overflow: hidden;
    color: #fff;
    padding: 0;
    text-align: right;
    margin: 0px 75px;

    transition: 1s;
}
nav.black ul {
    background: rgba(0, 0, 0, 0.5);
}
nav ul li {
    display: inline-block;
    padding: 20px;
}
nav ul li a {
    text-decoration: none;
    color:#333;
    font-size: 16px;
}
nav ul li a:hover{
    color: var(--primary-color);
   /* border-bottom: 1px solid var(--primary-color);*/
    transition: 1s;
}
.menu-icon {
    width: 100%;
    background: rgba(0, 0, 0, 0.5);
    text-align: right;
    box-sizing: border-box;
    padding: 15px 24px;
    cursor: pointer;
    color: #fff;
    display: none;
}
.logo-img{
  width:160px;
  height:30px;
}
@media(max-width: 800px) {
    .logo {

        top: 0;
        margin-top: 16px;

    float: left;
    margin: 16px 45px;
    color: #fff;
    font-weight: bold;
    font-size: 21px;

    }
    nav ul {
    list-style: none;
    background: rgba(0, 0, 0, 0);
    overflow: hidden;
    color: #fff;
    padding: 0;
    text-align: right;
    margin: 0px 30px;

    transition: 1s;
}
    nav ul li a {
    text-decoration: none;
    color:#333;
    font-size: 15px;
}
  .logo-img{
  width:120px;
  height:23px;
}

}
.floatingNav {
  /*width: calc(100vh - 100px); */
  box-shadow: 0px 1px 6px #999;
}
.main{
  margin: 20px 70px;
}
.hello{
  font-size: 18px;
  margin-bottom: 10px;
}

.totalinv {
  display: grid;
  grid-template-columns: 800px 400px;
  grid-gap: 10px;
  color: #444;
}
.box {
  background-color: #444;
  color: #fff;
  border-radius: 5px;
  padding: 20px;
  font-size: 150%;
  display: flex;
  margin-bottom: 20px;

}

.shift-small{
  padding-left:20px ;
}
.boxx{
  background-color: #444;
  color: #fff;
  border-radius: 5px;
  padding: 20px;
  font-size: 150%;
  display: flex;
}
.money{
  margin-left: 150px;
}
.shifter{
  margin-left: 240px;
}

@media(max-width: 800px) {

  .boxx{
  background-color: #444;
  color: #fff;
  border-radius: 5px;
  padding: 10px;
  font-size: 90%;
  display: block;
}

.main{
  margin: 0px 40px;
}
  .totalinv {
  display: block;
  grid-template-columns: 800px 400px;
  grid-gap: 10px;
  color: #444;
}
h3{
  font-size: 20px;
}
.shifter{
  margin-left: 0px;
  margin-top: 15px;
}
.money{
  margin-left: 80px;
}
.box {
  background-color: #444;
  color: #fff;
  border-radius: 5px;
  padding: 10px;
  font-size: 80%;
  display: block;
}
.money{
  margin-left: 20px;
}
}
.currentinv {
  display: grid;
  grid-template-columns: 400px 400px 400px;
  grid-gap: 10px;
  color: #444;
}

.box2 {
  background-color: #444;
  color: #fff;
  border-radius: 5px;
  padding: 20px;
  display: flex;
  font-size: 150%;
}
.left-small{
  margin-left: 90px;
}
@media(max-width: 800px) {
  .currentinv {
  display: block;
  grid-template-columns: 0px 0px 0px;
  color: #444;
}

.left-small{
  margin-left: 0px;
}

.box2 {
  background-color: #444;
  color: #fff;
  border-radius: 5px;
  padding: 20px;
  display: block;
  font-size: 80%;
  margin-bottom: 15px;
}
.down-small{
  margin-bottom: 13px;
}
.boxx{
  background-color: #444;
  color: #fff;
  border-radius: 5px;
  padding: 20px;
  font-size: 80%;
  display: block;
}
}
</style>
