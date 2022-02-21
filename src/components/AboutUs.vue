<template>
  <div id="aboutUs">
    <div class="about">
      <div class="up">
        <div class="img">
          <img src="../assets/new/imagethree.png" alt="">
        </div>
        <div class="text">
          <div class="titleUp">
            About Us
          </div>
          <div class="content">
            We are the world leading computing power exchange service provider. We have:
            <p>the 1st worldwide computing power exchange platform backboned by decentralized blockchain;</p>
            <p>tier 1 mature computing power relevant products ranked by Token Insight;</p>
            <p>stable and continuously growing customer base;</p>
            <p>comprehensive customer services related to computing power transactions;</p>
            <p>complete transaction ledger records on a world Top 100 public chains;</p>
            <p>internal stabilization mechanism to manage the exposures to volatilities of related
              cryptocurrency businesses.</p>
          </div>
        </div>
      </div>
      <div class="down">
        <div class="titleDown">
          Our Group Companies
        </div>
        <div class="cardList">
          <div class="card">
            <div class="content">
              <div class="name">SuperB Grace Ltd., the holding company and the global hashrate exchange platform
                operator.
              </div>
              <div class="address">
                <img src="../assets/address.png" alt="">
                <div class="addressName">Address: Unit 23D, United Centre, 95 Queensway, Hongkong</div>
              </div>
            </div>
          </div>
          <div class="card">
            <div class="content">
              <div class="name">Hainan Anmaiyun Web Technology Ltd., the wholly owned subsidiary of SuperB Grace Ltd.,
                and the R&D platform of our group.
              </div>
              <div class="address">
                <img src="../assets/address.png" alt="">
                <div class="addressName">Address: Room 3001, A17 Bld, Hainan Ecology Software Park, China.</div>
              </div>
            </div>
          </div>
          <div class="card">
            <div class="content">
              <div class="name">Hainan Anmaiyun Technology Ltd., the sales platform of our group in mainland China
                market.
              </div>
              <div class="address">
                <img src="../assets/address.png" alt="">
                <div class="addressName">Address: 45/F, No.1 Bld, IFS International Finance Center, Jinjiang District,
                  Chengdu, China.
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import {Component} from 'vue-property-decorator';

@Component
export default class About extends Vue {

}
</script>

<style lang="scss" scoped>
.about {
  width: 100vw;
}

.up {
  background: rgb(40, 40, 41);
  display: flex;
  padding: 7.39583vw 0;

  .img {
    width: 40.4167vw;
    height: 20.4167vw;
    overflow: hidden;

    img {
      width: 100%;
      height: 100%;
      display: block;
    }

    img:hover {
      transform: scale(1.2);
      transition: all 200ms ease-in-out;
    }
  }

  .content {
    p {
      margin-bottom: 0;
    }

    p::after {
      content: "";
      position: absolute;
      left: 0.104167vw;
      top: 0.729167vw;
      width: 0.208333vw;
      height: 0.208333vw;
      border-radius: 50%;
      background: rgb(255, 255, 255);
      border: 1px solid red;
    }
  }

  .text {
    margin-left: 6.77083vw;
    margin-right: 15vw;

    .titleUp {
      width: 9.11458vw;
      height: 1.5625vw;
      font-size: 1.875vw;
      font-weight: bold;
      color: rgb(255, 255, 255);
    }

    .content {
      margin-top: 3.07292vw;
      width: 31.9271vw;
      font-size: 1.04167vw;
      font-weight: 400;
      color: rgb(255, 255, 255);
      opacity: 0.71;
      line-height: 1.5625vw;
    }
  }
}

.down {
  margin-top: 4.01042vw;
  padding: 0px 18.8021vw;

  .titleDown {
    height: 1.66667vw;
    font-size: 1.5625vw;
    font-weight: bold;
    color: rgb(38, 38, 38);
    line-height: 3.64583vw;
  }

  .cardList {
    margin-top: 2.13542vw;
    @media screen and (max-width: 1400px) {
      .card {
        font-size: 1.04167vw;
      }
    }

    .card {
      margin-bottom: 1.66667vw;
      width: 62.1875vw;
      font-size: 0.833333vw;
      font-weight: 400;
      color: rgb(89, 89, 89);
      line-height: 1.5625vw;
      display: flex;
      background: rgba(238, 238, 238, 0.35);

      .content {
        flex: 1 1 0%;
        display: flex;
        flex-direction: column;
        -webkit-box-pack: center;
        justify-content: center;
        padding-left: 1.51042vw;
        position: relative;

        .address {
          display: flex;
          -webkit-box-pack: start;
          justify-content: flex-start;
          -webkit-box-align: center;
          align-items: center;
        }

        img {
          display: block;
        }
      }
    }

    .card::before {
      content: "";
      width: 0.260417vw;
      height: 4.53125vw;
      background: rgb(42, 138, 246);
    }
  }
}
</style>