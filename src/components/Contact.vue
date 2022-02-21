<template>
  <div class="contact">
    <div class="contactIcon">
      <img src="../assets/new/contact.png" alt="">
    </div>
    <div class="contain">
      <div class="description">SuperB Grace Ltd., the holding company of our group and the global computing power exchange service provider.</div>
      <div class="contactText">
        <span>Contact:</span>
        <div class="email">
          <span>Support@superbgrace.com</span>
        </div>
        <div class="site">
          <span>Unit 23D, United Centre, 95 Queensway, Hongkong</span>
        </div>
        <div class="tel">
          <span>400-0238-180 (Mainland China Only)</span>
          <div class="date">Mon.~Fri. 9:00-18:00(Beijing Time)</div>
        </div>
      </div>
      <div class="link">
        <span>Links:</span>
        <div class="item">
          <a href="https://www.rrmine.com" target="_blank">RRMine</a>
        </div>
        <div class="item">
          <a href="https://www.debay.io" target="_blank">DeBay</a>
        </div>
        <div class="item">
          <a href="https://www.renrenmine.com" target="_blank">renrenmine</a>
        </div>
        <div class="item">
          <a href="http://www.anmaicloud.com" target="_blank">AnmaiCloud</a>
        </div>
        <div class="item">
          <a href="https://bhpa.io" target="_blank">BHPA.io</a>
        </div>
        <div class="item">
          <a href="https://bhpay.io" target="_blank">BHPay</a>
        </div>
        <div class="item">
          <a href="https://bhpadvance.com" target="_blank">BHPA</a>
        </div>
      </div>
      <div class="Enterprise">
        <span>Enterprise registration number : </span>
        <span> 2371287</span>
      </div>
      <div class="copyright">
        ©2017-2019 SuperB Grace Limited.All Rights Reserved.
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import {Component} from 'vue-property-decorator';

@Component
export default class Contact extends Vue {

}
</script>

<style lang="scss" scoped>
  .contact {
    box-sizing: border-box;
    display: flex;
    flex-direction: column;
    -webkit-box-align: center;
    align-items: center;
    padding-top: 2.96875vw;
    position: relative;
    .contactIcon {
      position: absolute;
      right: 8.33333vw;
      top: 1.04167vw;
      cursor: pointer;
      > img {
        display: flex;
      }
    }
    .description {
      height: 0.9375vw;
      font-size: 0.9375vw;
      font-weight: 400;
      color: rgb(89, 89, 89);
      margin-bottom: 1.71875vw;
    }
    .contactText {
      height: 0.572917vw;
      font-size: 0.729167vw;
      font-weight: 400;
      color: rgb(89, 89, 89);
      display: flex;
      -webkit-box-align: center;
      align-items: center;
      margin-bottom: 1.30208vw;
      .email {
        margin-left: 2.60417vw;
        display: flex;
        -webkit-box-align: center;
        align-items: center;
      }
      .site {
        margin-left: 3.125vw;
        display: flex;
        -webkit-box-align: center;
        align-items: center;
      }
      .tel {
        margin-left: 2.60417vw;
        display: flex;
        -webkit-box-align: center;
        align-items: center;
        position: relative;
        .date {
          position: absolute;
          top: 100%;
          left: 0;
        }
      }
    }
    .link {
      height: 0.572917vw;
      font-size: 0.729167vw;
      font-weight: 400;
      color: rgb(89, 89, 89);
      display: flex;
      -webkit-box-align: center;
      align-items: center;
      margin-bottom: 1.25vw;
      >span {
        margin-right: 4.16667vw;
      }
      .item {
        margin-right: 1.82292vw;
      }
    }
    .Enterprise {
      height: 0.625vw;
      font-size: 0.729167vw;
      font-weight: 400;
      color: rgb(89, 89, 89);
      margin-bottom: 1.71875vw;
      >span {
        margin-right: 1.5625vw;
      }
    }
    .copyright {
      color: rgb(89, 89, 89);
      font-size: 0.729167vw;
      position: relative;
      padding-top: 1.14583vw;
      padding-bottom: 1.35417vw;
    }
    .copyright::before {
      content: "";
      width: 100%;
      height: 1px;
      position: absolute;
      top: 0;
      transform: translateX(-50 vw);
      background: rgb(238, 238, 238);
    }
  }
</style>