<template>
  <div>
    <Nav/>
    <div class="banner" id="Home">
      <a-carousel autoplay class="slider">
        <div>
          <div class="des">
            <img src="../assets/new/banner.png" alt="">
            <h3 class="title spe">
              Announcement：SuperB Grace Limited
              Stopped selling the computing power plans in Mainland China.
            </h3>
          </div>
        </div>
        <div>
          <div class="des">
            <img src="../assets/new/newbanner.jpeg" alt="">
            <h3 class="title">
              World Leading Computing Power Exchange Service Provider
            </h3>
          </div>
        </div>
      </a-carousel>

      <div class="section2">
        <div class="up">
          <div class="part1">
            <img src="../assets/new/imageone.png" alt="">
          </div>
          <div class="part2">
            <h3>Our Vision</h3>
            <span>To build a worldwide computing power exchange platform backboned by decentralized blockchain and to confront the challenges in the age of Big Data and Ai Robot</span>
          </div>
        </div>
        <div class="down">
          <div class="part3">
            <h3>Our Mission</h3>
            <span>
                To provide everyone easy and secured access to super computing power in a decentralized digital world
            </span>
          </div>
          <div class="part4">
            <img src="../assets/new/imagetwo.png" alt="">
          </div>
        </div>
      </div>
    </div>
    <AboutUs id="about"/>
    <BusinessView id="business"/>
    <History id="history"/>
    <EnterpriseDynamic id="dynamic"/>
    <Contact id="contact"/>
  </div>
</template>

<script>
import Vue from 'vue';
import 'ant-design-vue/dist/antd.css';
import About from '@/components/AboutUs.vue'
import {Component} from "vue-property-decorator";
import AboutUs from "@/components/AboutUs";
import BusinessView from "@/components/BusinessView";
import Contact from "@/components/Contact";
import EnterpriseDynamic from "@/components/EnterpriseDynamic";
import History from "@/components/History";
import Nav from "@/components/Nav";

@Component({
  components: {Nav, History, EnterpriseDynamic, Contact, BusinessView, AboutUs, About}
})
export default class Home extends Vue {
  cur = 0;

  // eslint-disable-next-line @typescript-eslint/explicit-module-boundary-types
  changeCur() {
    this.cur = this.active.cur;
    console.log(this.cur);
  }
}
</script>

<style lang="scss">
@import "~@/assets/style/reset.scss";

#Home {
  width: 100vw;
}

.ant-carousel > > > .slick-slide {
  text-align: center;
  height: 160px;
  line-height: 160px;
  background: #364d79;
  overflow: hidden;
}

.ant-carousel > > > .slick-slide h3 {
  color: #fff;
}

.ant-carousel .slick-list .slick-slide.slick-active {
  pointer-events: auto;
}

.slider {
  img {
    width: 100vw;
    top: 0;
    left: 0;
  }

  @media screen and (max-width: 1400px) {
    .des {
      font-size: 1.25vw;
      position: relative;
      .title {
        display: block;
        width: 61.0938vw;
        text-align: center;
        font-size: 3.125vw;
        font-weight: bold;
        height: 7.08333vw;
        line-height: 4.16667vw;
        color: rgb(255, 255, 255);
        position: absolute;
        inset: 0;
        margin: auto;
        z-index: 1;
      }
    }
  }
}

.section2 {
  display: flex;
  padding: 4.42708vw 18.75vw 4.63542vw;
  flex-wrap: wrap;

  .up {
    display: flex;

    img {
      display: block;
      width: 31.3542vw;
      height: 20.7812vw;
    }

    .part2 {
      padding: 3.22917vw 4.53125vw 5.78125vw 3.59375vw;
      background: rgb(250, 250, 250);
      height: 20.7812vw;

      h3 {
        color: rgb(38, 38, 38);
        width: 10.2083vw;
        height: 1.5625vw;
        margin-bottom: 3.75vw;
        font-weight: bold;
        font-size: 1.875vw;
      }

      span {
        width: 23.125vw;
        height: 6.45833vw;
        font-size: 1.5375vw;
        font-weight: 400;
        color: rgb(38, 38, 38);
        line-height: 1.875vw;
        opacity: 0.64;
        margin-left: 0;
      }
    }
  }

  .down {
    display: flex;

    img {
      display: block;
      width: 31.25vw;
      height: 17.1354vw;
    }

    .part3 {
      background: rgb(250, 250, 250);
      padding: 3.48958vw 5.05208vw 4.11458vw 3.22917vw;
      height: 17.1354vw;

      h3 {
        width: 11.7708vw;
        height: 1.5625vw;
        font-size: 1.875vw;
        font-weight: bold;
        color: rgb(42, 138, 246);
        margin-bottom: 3.38542vw;
      }

      span {
        width: 23.125vw;
        height: 4.58333vw;
        font-size: 1.5375vw;
        font-weight: 400;
        color: rgb(38, 38, 38);
        line-height: 1.875vw;
        opacity: 0.78;
      }
    }
  }
}

</style>