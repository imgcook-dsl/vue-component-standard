<template>
  <div class="page">
    <div class="mod1">
      <van-search
        class="block"
        placeholder="搜索商品、分类"
        shape="round"
      ></van-search>
      <img
        class="dian"
        src="https://img.alicdn.com/tfs/TB1iasNB7L0gK0jSZFtXXXQCXXa-45-45.png"
      />
    </div>
    <div class="mod2">
      <div class="block_3">
        <van-swipe class="block_2" autoplay="3000" indicator-color="fff">
          <van-swipe-item class="bannerWrap" v-for="(item, index) in loopData" :key="index">
            <img class="banner" src="https://img.alicdn.com/tfs/TB1iq.NB1L2gK0jSZPhXXahvXXa-690-345.png" />
          </van-swipe-item>
        </van-swipe>
      </div>
    </div>
    <swiper class="row" :options="swiperOption">
      <swiper-slide class="block_6" v-for="(item, index) in loopData" :key="index" >
        <img
          class="smallItem"
          src="https://img.alicdn.com/tfs/TB1oZ3RB4D1gK0jSZFKXXcJrVXa-144-144.png"
        />
        <span class="dragonBoatFestivalWelfare">端午福利</span>
      </swiper-slide>
    </swiper>
    <div class="mod3">
      <div class="block_8">
        <img class="jiaxigua" src="https://img.alicdn.com/tfs/TB1iKgSB4D1gK0jSZFyXXciOVXa-48-65.png" />
        <span class="hotRecommendation">热门推荐</span>
      </div>
      <div class="block_9">
        <span class="viewMore">查看更多</span>
        <img class="liveiconput" src="https://img.alicdn.com/tfs/TB1aXZOB.T1gK0jSZFrXXcNCXXa-21-38.png" />
      </div>
    </div>
    <div class="mod4">
      <div class="itemWrap" v-for="(item, index) in loopData" :key="index">
        <img class="item" src="https://img.alicdn.com/tfs/TB1hEkRBYY1gK0jSZTEXXXDQVXa-335-335.png" />
        <div class="priceWrap">
          <span class="title_2">杭州热销过千十大名茶…</span>
          <span class="rmb">¥</span> <span class="price">168</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      sliders: [1, 2],
      loopData: [1, 2],
      loopData: [1, 2, 3, 4],
      loopData: [1, 2, 3, 4],
      constants: {}
    };
  },
  methods: {}
};
</script>

<style scoped>
.page {
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  background-color: #f1f2f3;
  width: 750px;
  height: 1855px;
}

.mod1 {
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: row;
  justify-content: center;
  background-color: #d92c67;
  width: 750px;
  height: 97px;
}

.block {
  display: flex;
  align-items: center;
  flex-direction: row;
  margin-top: 22px;
  margin-right: 14px;
  border-radius: 31px;
  background-color: #ffffff;
  width: 647px;
  height: 62px;
}

.dian {
  margin-top: 38px;
  width: 30px;
  height: 30px;
}

.mod2 {
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: row;
  justify-content: center;
  box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.5);
  width: 750px;
  height: 414px;
}

.block_3 {
  display: flex;
  align-items: flex-start;
  flex-direction: row;
  justify-content: center;
  background-color: #d92c67;
  width: 750px;
  height: 414px;
}

.block_2 {
  display: flex;
  flex-direction: row;
  align-items: center;
  margin-top: 14px;
  width: 690px;
  height: 345px;
  overflow: hidden;
}

.bannerWrap {
  display: flex;
  align-items: center;
  flex-direction: row;
  justify-content: center;
  width: 690px;
  height: 345px;
}

.banner {
  width: 690px;
  height: 345px;
}

.row {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  width: 750px;
  height: 220px;
  position: relative;
  background-color: #ffffff;
}

.block_6 {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  margin-top: 7px;
  margin-right: 0;
  height: 141px;
}

.smallItem {
  position: relative;
  width: 96px;
  height: 96px;
}

.dragonBoatFestivalWelfare {
  position: relative;
  opacity: 1;
  margin-top: 8px;
  margin-left: 1px;
  line-height: 37px;
  white-space: nowrap;
  color: #4b4b4b;
  font-size: 26px;
  font-weight: 400;
}

.mod3 {
  box-sizing: border-box;
  display: flex;
  position: relative;
  align-items: center;
  align-self: center;
  flex-direction: row;
  justify-content: space-between;
  margin-top: 30px;
  padding-right: 1px;
  width: 688px;
  height: 46px;
}

.block_8 {
  display: flex;
  align-items: center;
  flex-direction: row;
  height: 46px;
}

.jiaxigua {
  margin-top: -3px;
  margin-right: 16px;
  width: 32px;
  height: 43px;
}

.hotRecommendation {
  opacity: 1;
  max-width: 285px;
  height: 45px;
  overflow: hidden;
  text-overflow: ellipsis;
  line-height: 45px;
  white-space: nowrap;
  color: #000000;
  font-size: 32px;
  font-weight: 600;
}

.block_9 {
  display: flex;
  align-items: center;
  flex-direction: row;
  height: 40px;
}

.viewMore {
  opacity: 1;
  margin-right: 8px;
  max-width: 249px;
  height: 40px;
  overflow: hidden;
  text-overflow: ellipsis;
  line-height: 40px;
  white-space: nowrap;
  color: #999999;
  font-size: 28px;
  font-weight: 400;
}

.liveiconput {
  width: 13px;
  height: 24px;
}

.mod4 {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: flex-start;
  flex-wrap: wrap;
  margin-top: 14px;
  margin-left: 29px;
  width: 710px;
  height: 997px;
  position: relative;
}

.itemWrap {
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: column;
  margin-top: 14px;
  margin-left: 2px;
  background-color: #ffffff;
  width: 335px;
  height: 480px;
}

.item {
  position: relative;
  width: 335px;
  height: 335px;
}

.priceWrap {
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: column;
  margin-top: 29px;
  margin-left: 10px;
  width: 308px;
  height: 106px;
}

.title_2 {
  position: relative;
  opacity: 1;
  line-height: 40px;
  white-space: nowrap;
  color: #333333;
  font-size: 28px;
  font-weight: 500;
}

.rmb {
  position: relative;
  opacity: 1;
  margin-top: 4px;
  max-width: 308px;
  height: 62px;
  overflow: hidden;
  text-overflow: ellipsis;
  line-height: 62px;
  white-space: nowrap;
  color: #d92c67;
  font-size: 44px;
  font-weight: 400;
}

.price {
  position: absolute;
  top: 44px;
  left: 26px;
  opacity: 1;
  line-height: 62px;
  white-space: nowrap;
  color: #d92c67;
  font-size: 44px;
  font-weight: 600;
}
</style>
