<template>
  <div id="history">
    <div class="history">
      <div class="titleHistory">Development History</div>
      <ul class="tabList">
        <li :class="{active: cur === 0}" @click="changeCur">Company Advancement Roadmap</li>
        <li :class="{active: cur === 1}" @click="changeCur">Technology Advancement Roadmap</li>
      </ul>
      <div class="historyContent" v-show="cur === 0">
        <div class="content">
          <div class="item item1">
            <div class="section">Aug 2017</div>
            <div class="description">Set up the company and introduced the version1.0 online platform.</div>
          </div>
          <div class="item item2">
            <div class="section">2018</div>
            <div class="description">Introduced the Node Plan, which set up twenty sales nodes covering China, Japan, Australia, USA and UK.</div>
          </div>
          <div class="item item3">
            <div class="section">June 2019</div>
            <div class="description">Restructured the company and the business model, upgrade the company from a hashrate retailer to a computing power network service provider, and new platform company has been introduced.</div>
          </div>
        </div>
        <img src="../assets/new/iconzz.png" alt="">
      </div>
      <div class="historyText" v-show="cur === 1">
        <div class="content1">
          <div class="item item1">
            <div class="section">Beginning of 2017</div>
            <div class="description">Explore the business model of the 'contracted electricity bill' and initiated the R&D of relevant blockchain technologies.</div>
          </div>
          <div class="item item2">
            <div class="section">Feb 2018</div>
            <div class="description">Participated the construction of global computing power network infrastructure and launched the world's first computing power public chain – BHP, which ranks top 100 among the world’s public chains.</div>
          </div>
          <div class="item item3">
            <div class="section">Nov 2019</div>
            <div class="description">Launched the world‘s first cross-chain computing power clearing and settlement system - RRP.</div>
          </div>
        </div>
        <img src="../assets/new/iconll.png" alt="">
        <div class="content2">
          <div class="item item1">
            <div class="section">Aug 2017</div>
            <div class="description">Launched the first 'all-inclusive' long-term hashrate contract product.</div>
          </div>
          <div class="item item2">
            <div class="section">Jun 2019</div>
            <div class="description">Launched the world's first decentralized computing power management & trading system - RRMine.</div>
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
export default class History extends Vue {
  cur = 0;
  // eslint-disable-next-line @typescript-eslint/explicit-module-boundary-types
  changeCur() {
    if( this.cur === 0) {
      this.cur = 1;
    } else {
      this.cur = 0;
    }
  }
}
</script>

<style lang="scss" scoped>
  .history {
    height: 40.9896vw;
    width: 100vw;
    background-image: url("../assets/new/bghh.png");
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
    flex-direction: column;
    -webkit-box-align: center;
    align-items: center;
    padding-top: 5vw;
    box-sizing: border-box;
    .titleHistory {
      width: 21.0417vw;
      height: 2.03125vw;
      font-size: 1.875vw;
      font-weight: bold;
      color: rgb(38, 38, 38);
    }
    .tabList {
      display: flex;
      margin-top: 2.08333vw;
      align-items: center;
      justify-content: center;
      .active {
        background: rgb(47, 47, 48);
        opacity: 1;
        color: rgb(255, 255, 255);
      }
      li {
        cursor: pointer;
        width: 18.4896vw;
        height: 3.22917vw;
        line-height: 3.22917vw;
        text-align: center;
        background: rgba(255, 255, 255, 0.1);
        border: 1px solid rgb(67, 67, 67);
        opacity: 0.3;
        font-size: 0.729167vw;
        font-weight: 400;
        color: rgb(38, 38, 38);
        margin-left: 1.51042vw;
      }
    }
    .historyContent {
      width: 62.1875vw;
      margin-top: 6.71875vw;
      .content {
        display: flex;
        margin-bottom: 1vw;
        .item1 {
          .description {
            width: 13.0208vw;
          }
        }
        .item2 {
          .description {
            width: 18.2292vw;
          }
        }
        .item3 {
          .description {
            width: 26.0417vw;
          }
        }
        .section {
          height: 0.625vw;
          font-size: 0.833333vw;
          font-weight: bold;
          color: rgb(38, 38, 38);
          margin-bottom: 1.25vw;
        }
        @media screen and (max-width: 1400px){
          .description {
            font-size: 1.04167vw;
          }
        }
        .description {
          height: 2.96875vw;
          font-size: 0.729167vw;
          font-weight: 400;
          color: rgb(89, 89, 89);
          line-height: 1.25vw;
          opacity: 0.46;
        }
      }
      img {
        width: 100%;
        display: block;
      }
    }
    .historyText {
      width: 62.1875vw;
      margin-top: 2.08333vw;
      @media screen and (max-width: 1400px){
        .description {
          font-size: 1.04167vw;
        }
      }
      .description {
        height: 2.96875vw;
        font-size: 0.729167vw;
        font-weight: 400;
        color: rgb(89, 89, 89);
        line-height: 1.25vw;
        opacity: 0.46;
      }
      .section {
        height: 0.625vw;
        font-size: 0.833333vw;
        font-weight: bold;
        color: rgb(38, 38, 38);
        margin-bottom: 1.25vw;
      }
      .content1 {
        width: 100%;
        display: flex;
        margin-bottom: 1.90625vw;
        .item1 {
          .description {
            width: 15.625vw;
          }
        }
        .item2 {
          .description {
            width: 23.4375vw;
          }
        }
        .item3 {
          margin-left: 7.08333vw;
          .description {
            width: 13.0729vw;
          }
        }
      }
      img {
        width: 100%;
        display: block;
      }
      .content2 {
        width: 100%;
        display: flex;
        margin-bottom: 3.90625vw;
        .item1 {
          margin-left: 10vw;
          .description {
            width: 15.625vw;
          }
        }
        .item2 {
          margin-left: 12vw;
          .description {
            width: 20.8333vw;
          }
        }
      }
    }
  }

</style>