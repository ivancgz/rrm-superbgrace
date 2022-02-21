<template>
  <div class="enterpriseDynamic">
    <div class="titleDynamic">Enterprise Dynamic</div>
    <div class="tabsBox">
      <div class="more">More ></div>
    </div>
    <div class="contentList">
      <a class="item" target="_blank">
        <div class="img">
          <img src="../assets/2020112601.jpg" alt="">
        </div>
        <div class="text">
          <div class="contentTitle">On BEYOND, Blockchain Industry Conference, RRMine Received 2020 IPFSs Most Influential Enterprise</div>
          <div class="content">On November 23-24, the "BEYOND·2020 Blockchain Industry Conference and Annual Awards Ceremony" hosted by Lieyunwang.com and Lieyun Finance was held in Shenzhen.</div>
          <div class="time">November 26, 2020</div>
        </div>
      </a>
      <a class="item" target="_blank">
        <div class="img">
          <img src="../assets/fuck1.jpg" alt="">
        </div>
        <div class="text">
          <div class="contentTitle">RRMine Was Invited by Juan Benet, The Founder of Filecoin, to Share "From IPFS to the New Digital Economic Value"</div>
          <div class="content">To celebrate the launch of Filecoin mainnet, the IPFS Protocol Lab team planned a week-long "Filecoin Liftoff Week" from October 19th to 23rd. The official Filecoin team, miners from the global community, scientists from all over the world, and IPFS ecological participants will gather together for a series of seminars and symposiums on different topics to discuss the future development of Filecoin.</div>
          <div class="time">October 23, 2020</div>
        </div>
      </a>
      <a class="item" target="_blank">
        <div class="img">
          <img src="../assets/new/news.jpg" alt="">
        </div>
        <div class="text">
          <div class="contentTitle">Board Secretary of Xnmatrix, Cecilia Ma, Delivered Keynote on Decentralized Cloud Computing During ABS2020</div>
          <div class="content">Cecilia Ma, the Board Secretary of XnMatrix, a leading decentralized cloud computing platform, delivered her insightful keynote titled "Battle without war: Decentralized Cloud Computing."</div>
          <div class="time">July 19, 2020</div>
        </div>
      </a>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import {Component} from 'vue-property-decorator';

@Component
export default class EnterpriseDynamic extends Vue {

}
</script>

<style lang="scss" scoped>
  .enterpriseDynamic {
    display: flex;
    flex-direction: column;
    -webkit-box-align: center;
    align-items: center;
    box-sizing: border-box;
    padding-top: 5.41667vw;
    padding-bottom: 4.375vw;
    background: rgb(248, 249, 251);
    .titleDynamic {
      height: 1.51042vw;
      font-size: 1.875vw;
      font-weight: bold;
      color: rgb(38, 38, 38);
      margin-bottom: 2.91667vw;
      }
    .tabsBox {
      width: 62.3958vw;
      display: flex;
      -webkit-box-pack: center;
      justify-content: center;
      -webkit-box-align: center;
      align-items: center;
      margin-bottom: 1.04167vw;
      position: relative;
      .more {
        position: absolute;
        font-size: 0.9375vw;
        font-weight: 400;
        right: 0;
        top: 50%;
        transform: translateY(-50%);
        color: rgb(137, 137, 137);
        cursor: pointer;
      }
    }
    .contentList {
      width: 62.5vw;
      .item {
        display: flex;
        background: rgb(255, 255, 255);
        padding: 1.5625vw 3.28125vw 1.61458vw 2.03125vw;
        margin-bottom: 1.25vw;
        .img {
          width: 12.5vw;
          height: 8.22917vw;
          overflow: hidden;
          margin-right: 1.66667vw;
          :hover {
            transform: scale(1.2);
            transition: all 200ms ease-in-out;
          }
          > img {
            display: block;
            width: 100%;
            height: 100%;
          }
        }
        .text {
          .contentTitle {
            width: 43.0208vw;
            height: 1.40625vw;
            line-height: 1.40625vw;
            overflow: hidden;
            text-overflow: ellipsis;
            font-size: 1.25vw;
            font-weight: 400;
            color: rgb(38, 38, 38);
            margin-bottom: 1.30208vw;
          }
          .contentTitle:hover {
            color: rgb(42,138,246);
          }
          @media screen and (max-width: 1400px){
            .content {
              font-size: 1.04167vw;
              line-height: 1.5625vw;
            }
          }
          .content {
            width: 43.8021vw;
            height: 3.125vw;
            overflow: hidden;
            text-overflow: ellipsis;
            font-size: 0.729167vw;
            font-weight: 400;
            color: rgb(89, 89, 89);
            line-height: 1.5625vw;
            margin-bottom: 1.25vw;
          }
          .time {
            height: 0.833333vw;
            font-size: 0.729167vw;
            font-weight: 400;
            color: rgb(153, 153, 153);
            line-height: 1.5625vw;
          }
        }
      }
      a {
        color: #000;
        text-decoration: none;
      }
    }
  }
</style>