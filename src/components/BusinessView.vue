<template>
  <div id="businessView">
    <div class="business">
      <div class="titleBusiness">Business View</div>
      <div class="description">Our technology breakthroughs enable us to build a decentralized Computing Power
        ecosystem
      </div>
      <div class="contain" style="top: 14.0625vw; left: 35.3646vw; width: 32.7083vw; height: 1.09375vw;">
        <img src="../assets/new/tech.png" alt="" class="icon">
        <p class="text">Support 3000 TPS Concurrent Distributed Network Technology</p>
      </div>
      <div class="contain" style="top: 20.2604vw;left: 25.0521vw;width: 18.9062vw;height: 0.833333vw;">
        <img src="../assets/new/link.png" alt="" class="icon">
        <p class="text">CP Cross-chain Real-time Settlement</p>
      </div>
      <div class="contain" style="top: 20.1562vw; left: 61.5625vw; width: 20.2604vw; height: 1.09375vw;">
        <img src="../assets/new/renzhen.png" alt="" class="icon">
        <p class="text">Multiple Smart Contract Authentication</p>
      </div>
      <div class="contain" style="top: 26.0417vw; left: 17.5vw; width: 21.0417vw; height: 2.39583vw;">
        <img src="../assets/new/xieyi.png" alt="" class="icon">
        <p class="text">Main Chain Anti-quantun Attack Security Protocal</p>
      </div>
      <div class="contain" style="top: 26.8229vw; left: 63.9583vw; width: 22.9688vw; height: 1.09375vw;">
        <img src="../assets/new/zichan.png" alt="" class="icon">
        <p class="text">Cross-chain Atomic Asset Exchange Protocol</p>
      </div>
      <div class="contain" style="top:32vw; left: 20vw; width: 15vw; height: 3vw;">
        <img src="../assets/new/yinsi.png" alt="" class="icon">
        <p class="text">Digital Identity Authentication and Privacy Protection</p>
      </div>
      <div class="contain" style="top: 32.9688vw; left: 64.2188vw; width: 18.9583vw; height: 1.09375vw;">
        <img src="../assets/new/offcenter.png" alt="" class="icon">
        <p class="text">Decentralized Secure Trading Ledger</p>
      </div>
    </div>
    <div class="layout">
      <div class="titleLayout">Global Layout</div>
      <div class="description">200 employees over 10 branches and offices around the world</div>
      <div class="imgBox">
        <div class="show">
          <div class="contentBox">
            <div id="imgContent" style="left: 0vw; transition: all 0.3s ease 0s;">
              <img id="img" ref="image" :src="item.src" alt="" v-for="item in imageBox" :key="item.id">
            </div>
            <div id="imgContent2" style="left: 100vw; transition: all 0.3s ease 0s;">
              <img id="img2" ref="image" :src="item.src" alt="" v-for="item in imageBox" :key="item.id">
            </div>
          </div>
          <div class="arrow" @click="nextImg">
            <img src='../assets/new/rightarrow.png' alt="">
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="js">
import Vue from 'vue';
import {Component} from 'vue-property-decorator';

@Component
export default class BusinessView extends Vue {
  // eslint-disable-next-line @typescript-eslint/explicit-module-boundary-types
  data() {
    return {
      imageBox: [
        {id: 1, src: require('../assets/new/icone.png')},
        {id: 2, src: require('../assets/new/iconp.png')},
        {id: 3, src: require('../assets/new/iconq.png')},
        {id: 4, src: require('../assets/new/iconr.png')},
        {id: 5, src: require('../assets/new/icont.png')},
        {id: 6, src: require('../assets/new/iconu.png')},
        {id: 7, src: require('../assets/new/iconw.png')},
        {id: 8, src: require('../assets/new/icony.png')}
      ],
    }
  }

  // eslint-disable-next-line @typescript-eslint/explicit-module-boundary-types
  nextImg() {
    let image = document.getElementById("imgContent")
    let image2 = document.getElementById("imgContent2")

    if (image.style.left === '0vw') {
      image.style.left = '-12.5vw';
      image.style.transition = 'all 0.3s ease 0s'
    } else if (image.style.left === '-12.5vw') {
      image.style.left = '-25vw'
    } else if (image.style.left === '-25vw') {
      image.style.left = '-37.5vw'
    } else if (image.style.left === '-37.5vw') {
      image.style.left = '-50vw'
    } else if (image.style.left === '-50vw') {
      image.style.left = '-62.5vw'
    } else if (image.style.left === '-62.5vw') {
      image.style.left = '-75vw'
    } else if (image.style.left === '-75vw') {
      image.style.left = '-87.5vw'
    } else if (image.style.left === '-87.5vw') {
      image.style.left = '-100vw'
      if (image.style.left === '-100vw') {
        image.style.left = '0vw'
        image.style.transition = 'all 0s ease 0s'
      }
    }

    if (image2.style.left === '100vw') {
      image2.style.left = '87.5vw'
      image2.style.transition = 'all 0.3s ease 0s'
    } else if (image2.style.left === '87.5vw') {
      image2.style.left = '75vw'
    } else if (image2.style.left === '75vw') {
      image2.style.left = '62.5vw'
    } else if (image2.style.left === '62.5vw') {
      image2.style.left = '50vw'
    } else if (image2.style.left === '50vw') {
      image2.style.left = '37.5vw'
    } else if (image2.style.left === '37.5vw') {
      image2.style.left = '25vw'
    } else if (image2.style.left === '25vw') {
      image2.style.left = '12.5vw';
    } else if (image2.style.left === '12.5vw') {
      image2.style.left = '0vw'
      if (image2.style.left === '0vw') {
        image2.style.left = '100vw'
        image2.style.transition = 'all 0s ease 0s'
      }
    }
  }
}
</script>

<style lang="scss" scoped>
#businessView {
  width: 100vw;
}

.business {
  display: flex;
  flex-direction: column;
  -webkit-box-align: center;
  align-items: center;
  box-sizing: border-box;
  padding-top: 4.11458vw;
  height: 39.3229vw;
  background-image: url("../assets/new/bgnn.png");
  background-position: center bottom;
  background-repeat: no-repeat;
  background-size: contain;
  position: relative;

  .titleBusiness {
    width: 13.75vw;
    height: 1.5625vw;
    font-size: 1.875vw;
    font-weight: bold;
    color: rgb(42, 138, 246);
  }

  @media screen and (max-width: 1400px) {
    .description {
      font-size: 1.25vw;
    }
  }

  .description {
    margin-top: 1.30208vw;
    height: 1.09375vw;
    font-size: 1.25vw;
    font-weight: 300;
    color: rgb(38, 38, 38);
  }

  .contain {
    display: flex;
    -webkit-box-align: center;
    align-items: center;
    position: absolute;

    p {
      margin-bottom: 0;
    }

    .icon {
      //width: 1.30208vw;
      width: 1.30208vw;
      display: block;
      margin-right: 0.364583vw;
    }

    @media screen and (max-width: 1400px) {
      .text {
        font-size: 1.04167vw;
      }
    }

    .text {
      font-size: 0.9375vw;
      font-weight: 400;
      color: rgb(89, 89, 89);
    }
  }
}

.layout {
  display: flex;
  flex-wrap: wrap;
  flex-direction: column;
  -webkit-box-align: center;
  align-items: center;
  height: 56.3021vw;
  box-sizing: border-box;
  padding-top: 4.16667vw;
  background-image: url("../assets/new/bgk.png");
  background-repeat: no-repeat;
  background-size: auto;
  position: relative;

  .titleLayout {
    height: 2.03125vw;
    font-size: 1.875vw;
    font-weight: bold;
    color: rgb(255, 255, 255);
    margin-bottom: 1.35417vw;
  }

  .description {
    height: 1.40625vw;
    font-size: 1.25vw;
    font-weight: 400;
    color: rgba(255, 255, 255, 0.77);
    margin-bottom: 5.41667vw;
  }

  .imgBox {
    width: 100vw;
    height: 7.39583vw;
    position: absolute;
    bottom: 5vw;
    left: 0;

    .show {
      position: relative;
      display: flex;
      justify-content: center;
      align-items: center;

      .contentBox {
        width: 48.75vw;
        height: 7.39583vw;
        overflow: hidden;
        position: relative;

        #imgContent {
          position: absolute;
          height: 7.39583vw;
          display: flex;
          width: 100vw;

          #img {
            margin-right: 1.51042vw;
          }
        }

        #imgContent2 {
          position: absolute;
          height: 7.39583vw;
          display: flex;
          width: 100vw;

          #img2 {
            margin-right: 1.51042vw;
          }
        }

        > img {
          width: 11.0417vw;
          height: 7.39583vw;
          margin-right: 1.51042vw;
        }
      }

      .arrow {
        position: absolute;
        right: 21.0188vw;
        top: 50%;
        transform: translateY(-50%);
        width: 2.86458vw;
        height: 3.80208vw;
        background: rgba(248, 248, 248, 0.12);
        border-radius: 0.104167vw;
        display: flex;
        -webkit-box-pack: center;
        justify-content: center;
        -webkit-box-align: center;
        align-items: center;
        cursor: pointer;
      }

      .arrow:hover {
        background: rgba(248, 248, 248, 0.22);
      }
    }
  }
}
</style>