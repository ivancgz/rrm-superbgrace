<template>
  <div>
    <div id="nav">
      <div class="logo">
        <img src="../assets/logo.png" alt="優采有限公司" @click="print(titleBox)">
      </div>
      <ul class="nav" >
        <li v-for="(item, index) in titleBox" :key="index" :class="selectedIndex === index ? 'active':''" @click="getTitle(index, item.titleBox)">
          <a :href="item.href">{{item.name}}</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script lang="js">
export default  {
  // eslint-disable-next-line @typescript-eslint/explicit-module-boundary-types
  data() {
    return {
      selectedIndex: 0,
      titleBox: [
        { id: 0, href: '#Home', name: 'Home' },
        { id: 1, href: '#about', name: 'About Us', },
        { id: 2, href: '#business', name: 'Business View', },
        { id: 3, href: '#history', name: 'History', },
        { id: 4, href: '#dynamic', name: 'Enterprise Dynamic', },
        { id: 5, href: '#contact', name: 'Contact', }
      ]
    }
  },
  methods: {
    // eslint-disable-next-line @typescript-eslint/explicit-module-boundary-types
    getTitle(index) {
    this.selectedIndex = index;
    },
    // eslint-disable-next-line @typescript-eslint/explicit-module-boundary-types
    print(titleBox) {
      console.log(titleBox);
     }
  }


}
</script>

<style lang="scss" scoped>
#nav {
  position: fixed;
  padding: 0 18.4896vw;
  height: 3.64583vw;
  background: black;
  z-index: 10;
  width: 100vw;
  display: flex;
  align-items: center;
  justify-content: space-between;

  .nav {
    list-style: none;
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-bottom: 0;

    .active > a {
      color: #2A8AF6;
    }

    > li > a {
      margin-left: 2.39583vw;
      font-weight: 400;
      font-size: 1.04167vw;
    }
    > li > a:hover {
      color: #2A8AF6;
    }
  }

  .logo > img {
    width: 100%;
    display: block;
  }

  img {
    vertical-align: middle;
  }

  a {
    color: white;
    outline: none;
    background-color: transparent;
    cursor: pointer;
  }

  a:active {
    color: #2A8AF6;
    //border-bottom: 1px solid #2A8AF6;
    //height: 1px;
    content: "";
    width: 2.03125vw;
    height: 0.104167vw;
    bottom: -0.416667vw;
    left: 50%;
    transform: translateX(-50%);
  }

  a:hover, a:focus {
    outline: 0;
  }
}
</style>