<template>
  <div class="page">
    <div class="bidpage-content">
    <div class="page__header header">
        <div class="header__graybox">
        <div class="logo"></div> <img src='~images/star.png' alt="about us">THEYALOW
        <div class="graybox header__graybox graybox__smalltext">Craft&nbsp;By&nbsp;Css&nbsp;author.com</div>
        </div>
        <div class="yellowbox-container">
        <div class="header__yellowbox yellowbox-container__yellowbox yellowbox-container__yellowbox--about">
          <img src='~images/man-icon.png' alt="about us">
          <span class="yellowbox__text">ABOUT US</span>
          </div>
        <div class="header__yellowbox yellowbox-container__yellowbox yellowbox-container__yellowbox--services">
          <img src='~images/key-icon.png' alt="services">
          <span class="yellowbox__text">SERVICES</span></div>
        <div class="header__yellowbox yellowbox-container__yellowbox yellowbox-container__yellowbox--contact">
          <img src='~images/email-icon.png' alt="contact">
          <span class="yellowbox__text">CONTACT</span></div>
           <div class="rightbox__ghost"></div>
        </div>
    </div>
    <div class="page__videoplayer videoplayer">
      <div class="videoplayer__arrow videoplayer__arrow--left"></div>
      <div class="videoplayer__window"></div>
      <div class="videoplayer__description">The Cool<br><div class="videoplayer__description videoplayer__description--white">The minimal</div></div>
        <div class="videoplayer__arrow videoplayer__arrow--right"></div>
      </div>
    </div>
      <div class="page__submenu submenu">
        <div class="submenu__box box">
          <img src='~images/download-icon.png' class="box__pic" alt="design">
          <div>BETTER DESIGHN</div>
        </div>
         <div class="submenu__box box">
          <img src='~images/leaf-icon.png' class="box__pic box__pic--leaf" alt="cusmomise">
          <div>CUSTOMISE</div>
        </div>
         <div class="submenu__box box">
          <img src='~images/plane-icon.png' class="box__pic box__pic--plane" alt="free">
          <div>ITS FREE</div>
        </div>
      </div>
      <div class="page__whitebox whitebox">
        <div class="whitebox__whitetext">Lorem ipsum dolor sit amet</div>
        <div class="whitebox__flexbox">
         <div class="whitebox__orangebox orangebox">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut
           <div class="orangebox__plus orangebox__plus--1">+</div>
         </div>
         <div class="orangebox__monkey"><img src='~images/monkey.png' class="orangebox__monkey" alt="monkey"></div>
         <div class="whitebox__tweet"><img src='~images/twitter.png' class="" alt="twitter">
         <div class="tweet tweet__twentytwo">22</div>
           <div class="orangebox__plus">+</div>
         </div>
        </div>
        <div class="whitebox__april april"><div class="april__text april__text--twentyfive">25</div><span class="april__text"> april</span></div>
        <div><img src='~images/scroll.png' class="whitebox__scroll" alt="scroll"></div>
      </div>
      <div class="page__orangebigbox orangebigbox">
        <div class="orangebigbox__pic"><img src='~images/twitter.png' class="" alt="twitter"></div>
         <div class="orangebigbox__rightbox rightbox">
           <img class="rightbox__pic" src='~images/whitequote.png' alt="twitter"><div class="pic__text pic__text--1">Daily Mobile UI Design Inspiration #1<br>
via @cssauthor </div>
           <img class="rightbox__pic" src='~images/yellowquote.png' alt="twitter"><div class="pic__text pic__text--2">Daily Mobile UI Design Inspiration #1<br>
via @cssauthor</div>
            <img class="rightbox__pic" src='~images/orangequote.png' alt="twitter"><div class="pic__text pic__text--3">Daily Mobile UI Design Inspiration #1<br>
via @cssauthor</div>
            <div><input class="input"><button class="btn">Tweet</button></div>
           </div>
      </div>
      <div class="page__darkbox darkbox">
      <div class="darkbox__text">Lorem ipsum dolor sit amet</div>
      <img src='~images/comps.png' alt='Lorem'>
      </div>
      <div class="page__smalldarkbox smalldarkbox">
         <div class="smalldarkbox__text"><img src='~images/star.png' alt="star"><div class="logo-text">THEYALOW</div></div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'Page'
}
</script>
<style lang="scss" scoped>
.page{
  margin: 0 auto;
  width: 640px;
  height: 90px;
  background-color: gray;
  &__videoplayer{
  width: 100%;
  }
}
.videoplayer{
  height: 325px;
  &__arrow{
     visibility: hidden;
  }
  &__window {
    width: 100%;
    height: 325px;
    background-image: url('~images/videoplayer.png')
  }
  &__description {
    visibility: hidden;
  }
}
.submenu {
  display: flex;
  flex-flow: row nowrap;
  width: 640px;
  height: 169px;
  background-image: url('~images/bg-gray.png');
  justify-content: space-around
}
.header{
  display: flex;
  flex-flow: row nowrap;
  &__graybox {
    display: flex;
    align-items: center;
    font-family: 'LucidaSansItalic';
    font-weight: 300;
    font-style: italic;
    font-size: 20px;
    color: white;
    width: 185px;
    height: 90px;
    background-image: repeating-linear-gradient(to top,rgb(128, 128, 128) 0%,rgb(91, 91, 91) 98.2%,rgb(91, 91, 91) 98.2%,rgb(169, 169, 169) 100%);
    }
  &__yellowbox{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 172px;
    border-left: 1px #d6ac05 solid;
    background-image: url('~images/bg-yellow.png');
    color: #9b7d08;
    }
.yellowbox{
  &__text{
    padding-left: 10px;
    z-index: 1;
  }
}
.yellowbox-container {
  display: flex;
  justify-content: center;
  width: 455px;
  &__yellowbox{
    &--about{
      width: 171px;
    }
    &__services {
      width: 131px;
    }
    &__contact{
      width: 147px;
    }
  }
}
.graybox{
&__smalltext{
  visibility: hidden;
  font-size: 13px;
  text-transform: uppercase;
  position: relative;
  top: 9px;
  width: auto;
}
}
}
.logo {
display: none;
width: 40px;
height: 39px;
background-image: url('~images/star.png');
background-repeat: no-repeat
}

.box{
  display: flex;
  flex-flow: column nowrap;
  align-items: center;
  justify-content: center;
  width: 170px;
  &__pic{
    width: 89px;
    height: 61px;
    padding-bottom: 22px;
    &--leaf{
      width: 67px;
      height: 69px;
    }
    &--plane{
      width: 68px;
      height: 69px;
    }
  }
}
.whitebox{
  height: 232px;
  font-size: 29px;
  background-color: white;
  &__flexbox{
    display: flex;
    flex-flow: row nowrap;
    justify-content: normal;
    align-content: center;
  }
  &__orangebox{
    font-size: 29px;
  }
  &__tweet{
    visibility: hidden;
  }
  &__whitetext{
    visibility: hidden;
    height: 0;
    font-size: 28px;
    text-align: left;
  }
  &__scroll{
    visibility: hidden;
    padding-top: 50px;
  }
}
.april {
  visibility: hidden;
}
.orangebigbox {
  width: 100%;
  height: 230px;
  background-color: #f5c507;
  display: flex;
  flex-flow: row nowrap;
  &__pic{
    padding-left: 86px;
    padding-top: 54px;
  }
  &__rightbox{
    display: flex;
    flex-flow: column;
    justify-content: start;
    padding-top: 24px;
    padding-left: 105px;
    &__ghost {
      position: relative;
      top: 52px;
      right: 480px;
      z-index: 0;
      background-image: url('~images/transparent-menu.png')
    }
  }
}
.orangebox{
  padding: 7px;
  background-color: #ec9e03;
  min-width: 305px;
  height: 218px;
  font-size: 29px;
  color: white;
  &__plus{
    visibility: hidden;
    text-align: right;
    font-size: 20px;
    font-weight: 700;
    position: relative;
    bottom: 10px;
  }
  &__monkey{
    width: 321px;
    height: 232px;
  }
}
.rightbox{
  &__pic{
    height: 42px;
  }
}
.input{
  width: 200px;
  height: 27px;
  border-radius: 15px 0px 0px 15px;
}
.btn{
  border-radius: 0px 15px 15px 0px;
  width: 67px;
  height: 34px;
  background: linear-gradient(to bottom, #e9a826 0%,#d08f0c 100%);
  color: white;
  font-size: 15px;
  border: 2px #d0a806 solid;
}
.pic__text{
    height: 10px;
    &--1{
    position: relative;
    top: -40px;
    left: 0px;
    width: 100%;
    }
    &--2{
    position: relative;
    top: -40px;
    left: 0px;
    width: 100%;
    }
    &--3{
    position: relative;
    top: -40px;
    left: 0px;
    width: 100%;
}
}
.darkbox{
  width: 100%;
  height: 462px;
  background-color: #474747;
  background-image: url('~images/bg-dark-gray.png');
  &__text{
    color: #f5c506;
    text-transform: uppercase;
    letter-spacing: 0.1px;
    font-size: 39px;
    padding-top: 36px;
  }
}
.smalldarkbox{
  width: 100%;
  height: 40px;
  display: flex;
  background-color: #474747;
  align-items: center;
  font-family: 'LucidaSansItalic';
  font-weight: 300;
  font-style: italic;
  font-size: 20px;
  color: white;
  box-shadow: 0 0 10px rgba(0,0,0,0.5);
  &__text{
    padding-left: 30px;
    display: flex;
    flex-flow: row;
    align-items: center;
  }
}

@media (min-width: 641px) {
  .page{
    margin: 0 auto;
    width: 1295px;
  }
  .bidpage-content {
    height: 557px;
    background-image: url('~images/bg-header-pc.png');
  }
  .header {
    &__yellowbox{
      position: relative;
      top: 60px;
      left: 60px;
      height: 40px;
      background: #f5c506;
      border: transparent;
      color: #9b7d08;
    }
    &__graybox{
      padding-left: 145px;
      padding-top: 24px;
      background-color: transparent;
      background-image: none;
      font-size: 45px;
      width: AUTO;
      img {
        width: 72px;
        height: 69px;
      }
     }
  .graybox {
    &__smalltext{
      visibility: visible;
      font-size: 13px;
      text-transform: uppercase;
      padding-left: 0;
      font-style: normal;
      position: relative;
      top: 0px;
      }
    }
  }
  .logo{
    width: 83px;
    height: 83px;
    background-image: url('~images/star_big.png');
  }
.rightbox__ghost {
    display: block;
    width: 500px;
    height: 49px;
    position: relative;
    z-index: 0;
    top: 51px;
    right: 355px;
    background-image: url('~images/transparent-menu.png')
    }
  .yellowbox-container {
    display: flex;
    justify-content: center;
    min-width: 855px;
    margin-left: 60px;
    &__yellowbox{
      &--about{
        width: 171px;
        z-index: 1;
      }
      &--services {
        width: 131px;
        z-index: 1;
      }
      &--contact{
        width: 147px;
        z-index: 1;
      }
    }
  }
  .videoplayer {
    display: flex;
    flex-flow: row nowrap;
    justify-content: space-between;
    padding: 50px 0;
    align-items: center;
    padding: 50px 0;
    &__arrow{
      visibility: visible;
      width: 32px;
      height: 57px;
      &--left{
        background-image: url('~images/arrow.png');
      }
      &--right{
        background-image: url('~images/arrow2.png');
      }
    }
    &__window {
      width: 550px;
      background-image: url('~images/player.png');
    }
    &__description{
      visibility: visible;
      font-size: 60px;
      text-transform: uppercase;
      font-weight: 500;
      color: #f5c506;
      &--white{
      position: relative;
      left: 0px;
      top: 0px;
      color: white;
      }
    }
  }
  .submenu {
  display: flex;
  flex-flow: row nowrap;
  width: 100%;
  height: 210px;
  background-image: url('~images/bg-white.png');
  justify-content: center;
  font-size: 26px;
  box-shadow: 10px rgba(0,0,0,0.5);
}
.box{
  display: flex;
  flex-flow: column nowrap;
  align-items: center;
  justify-content: center;
  width: 380px;
  border: 1px #d3d3d3 solid;
  &__pic{
    width: 109px;
    height: 74px;
    padding-bottom: 22px;
    &--leaf{
      width: 91px;
      height: 95px;
    }
    &--plane{
      width: 81px;
      height: 83px;
    }
  }
}
.whitebox {
  height: 300px;
  background-image: url('~images/bg-orange.png');
  padding: 105px 118px;
  &__tweet{
    visibility: visible;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 337px;
    height: 233px;
    background-color: #ec9e03;
  }
  &__whitetext{
    visibility: visible;
    height: 0;
    color: white;
    text-transform: uppercase;
    font-size: 32px;
    position: relative;
    bottom: 70px;
  }
  &__scroll{
    visibility: visible;
    display: flex;
    justify-content: center;
  }
}
.tweet{
  font-size: 29px;
  color: white;
  text-align: right;
  font-size: 20px;
  &__twentytwo{
    position: relative;
    bottom: 90px;
    left: 50px;
}
}
.pic__text{
  display: none;
}
.orangebigbox{
  display: none;
}
.april {
  visibility: visible;
  background-color: #ddb101;
  width: 112px;
  height: 85px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-flow: column;
  font-weight: bolder;
  ;
  &__text{
    color: #ba7321;
    font-size: 18px;
    text-transform: uppercase;
    font-weight: 500;
    &--twentyfive{
      line-height: 50px;
      color: white;
      font-size: 50px;
    }
  }
}
.orangebox{
  font-size: 29px;
  width: 288px;
  text-align: left;
  font-weight: 100;
  padding-left: 20px;
   &__plus {
    visibility: visible;
    position: relative;
    top: 90px;
    left: 50px;
    font-weight: 700;
    color: white;
    &--1{
      top: 0px;
      left: 0px;
      }
    }
  }
  .rightbox{
    width: 284px;
  }
}
</style>
