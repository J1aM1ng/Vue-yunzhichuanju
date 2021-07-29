<template>
  <div class="home">
    <div class="carousel">
      <el-carousel :interval="4000"
                   type="card"
                   height="imageHeight">
        <el-carousel-item v-for="item in imgList"
                          :key="item.id">
          <el-row>
            <el-col :span="24"><img ref="imgHeight"
                   :src="item.imageUrl"
                   class="banner_img" /></el-col>
          </el-row>
        </el-carousel-item>
      </el-carousel>
    </div><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />

    <div class="content">
      <div class="first">
        <div class="text">
          <p>突出产品特色，实现人机互动。软硬件先进，外观设计美观</p>
          <div class="button">
            <el-button type="primary"
                       plain>了解更多</el-button>
          </div>
        </div>
        <img src="../assets/images/first1.png"
             alt="images"
             id="first1" />
      </div><br /><br /><br />

      <!-- <div class="second">
        <img src="../assets/images/first2.png"
             alt="images"
             id="first2" />
        <div class="text">
          <strong>厦门大学 研究生支教团</strong><br /><br />
          <small>厦门大学研究生支教团</small>
          <p>闽宁协作的二十多年间，厦门大学研究生支教团也从祖国东南沿海到西北，
            用知识打开孩子们通往世界的窗户，用青春为孩子们的求学路助力。
            研究生支教团的队员，都是厦门大学大四的毕业生，在宁夏支教一年后再回校读研，
            大家的平均年龄22岁，正值青春年华，对于支教都充满了热情。
          </p>
          <div class="button">
            <el-button type="primary"
                       plain>了解更多</el-button>
          </div>
        </div>
      </div> -->
    </div>

    <el-footer>
      <p id="midStrong">E智驱售</p>
      <small>专注于商用服务机器人研发</small><br /><br />
      <div class="button">
        <el-button type="primary"
                   plain
                   class="midButton">了解更多</el-button>
      </div>
    </el-footer>

    <el-main>
      <div class="main">
        <img src="../assets/logo.png"
             alt=""
             id="footLogo"><br />
        <p>机器人行业探索者,专注于商用服务机器人研发。产品涉及酒店机器人、迎宾机器人、讲解机器人、送餐机器人、机器人底盘等</p>
        <br /><br /><br />
        <p style="font-size: 20px;color: white;">北京公司（总部）</p>
        <p>北京市海淀区新中关大厦B5107</p>
      </div>
    </el-main>

  </div>
</template>

<style scoped>
.home {
  position: relative;
}

.content {
  width: 70%;
  position: absolute;
  left: 50%;
  top: 55%;
  transform: translate(-50%, -50%);
}

.mid {
  padding: 100px;
  min-height: 600px;
  position: relative;
}

.text {
  display: inline-block;
  position: relative;
  width: 50%;
  text-align: left;
}
.el-carousel__item h3 {
  color: #475669;
  font-size: 14px;
  opacity: 0.75;
  line-height: 200px;
  margin: 0;
}

.el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n + 1) {
  background-color: #d3dce6;
}

.el-footer {
  background-color: #434446;
  color: rgb(247, 238, 238);
  text-align: center;
  position: relative;
  top: 600px;
  min-height: 250px;
  padding: 30px;
}

.el-main {
  background-color: #242425;
  color: rgb(247, 238, 238);
  text-align: left;
  min-height: 400px;
  padding: 30px;
  padding-left: 10%;
  position: relative;
  top: 600px;
  display: flex;
  justify-content: center;
  flex-flow: row;
  overflow: hidden;
}

.left {
  width: 300px; /*固定宽度*/
}

.center {
  flex: 1; /*这里设置为占比1，填充满剩余空间*/
  text-align: center;
}

.right {
  width: 300px;
}

.center,
.right {
  position: relative;
  top: 50px;
}

.carousel {
  margin: 20px;
  margin-bottom: 100px;
}

.button {
  position: absolute;
  left: 40%;
  transform: (-50%);
}

#first1 {
  width: 450px;
  height: 240px;
  display: inline-block;
  position: relative;
  top: 50px;
  left: 30px;
}

#first2 {
  width: 450px;
  height: 240px;
  display: inline-block;
  position: relative;
  top: 50px;
  left: 30px;
  margin-right: 50px;
}

.first .second {
  padding: 30px;
}

#midStrong {
  font-size: 200%;
}

.midButton {
  position: relative;
  left: 100px;
}

.main {
  color: white;
  text-align: center;
  transform: translate(-6%, 0);
}

#footLogo {
  width: 100px;
  height: 100px;
}
</style>

<script>
export default {
  name: 'Home',
  data () {
    return {
      imgList: [
        { id: 0, imageUrl: require('../assets/images/banner1.png') },
        { id: 1, imageUrl: require('../assets/images/banner2.png') },
        { id: 2, imageUrl: require('../assets/images/banner3.png') },
      ]
    }
  }
}
</script>
