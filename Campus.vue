<!-- 掌大带你看校园 -->

<template>
  <div class="all">

    <!-- 第一部分 -->
    <div class="nav" v-for="item in naMe">
      <div class="nav_1">

        <div class="nav_1_in">
          <img :src="item.logo">
          <p>{{item.name}}</p>
        </div>
      </div>

      <p class="tex">{{item.title}}</p>

      <div class="im"><img :src="item.src"></div>

    </div>

    <!-- 第二部分 -->

    <!-- <div class="nav">
      <div class="nav_1">

        <div class="nav_1_in">
        	<img :src="item.src" v-for="item in loGo" :key="item.id">
        	<p v-for="item in naMe">{{item.name}}</p>
        </div>

   

      </div>

      <p class="tex"><a style="font-weight: 800;">[科普]</a>&nbsp POP&nbsp从音符到笔触</p>

      <span class="im2"><img src="../assets/images/banner2.png" alt="" srcset=""></span>

    </div> -->

    <!-- 第三部分 -->

    <div class="nav" style=" padding-bottom: 15%;">
      <div class="nav_1">

        <div class="nav_1_in">
          <img :src="item.src" v-for="item in loGo" :key="item.id">
          <p v-for="item in naMe">{{item.name}}</p>
        </div>

      </div>

      <p class="tex">一所伟大的学校,无论是闹鬼,老师死亡,学生遇难,校长被杀,都不能阻止他每年按时开学</p>

      <div class="item3">
        <img :src="item.src" v-for="item in imgLis" :key="item.id">
      </div>

    </div>

    <!-- 底部广告 -->

    <div class="foot">

      <!-- <img src="../assets/images/logo2.png" alt="" srcset=""> -->
      <h2>掌上大学</h2>
      <div class="footer">
        <a style="color:#ffdf08;">打开</a>
        <a style="color:#0a0003; background-color: #ffdf08;">下载</a>
      </div>
      <p>新校园生活方式</p>
    </div>

  </div>

</template>

<script>
//导出
export default {
  data () {
    return {
      // require
      imgLis: [
        { id: 1, src: require('../assets/images/1960698591-(1)_03.png') },
        { id: 2, src: require('../assets/images/1960698591-(1)_05.png') },
        { id: 3, src: require('../assets/images/1960698591-(1)_07.png') },
        { id: 4, src: require('../assets/images/1960698591-(1)_12.png') },
        { id: 5, src: require('../assets/images/1960698591-(1)_13.png') },
        { id: 6, src: require('../assets/images/1960698591-(1)_14.png') },
        { id: 7, src: require('../assets/images/1960698591-(1)_18.png') },
        { id: 8, src: require('../assets/images/1960698591-(1)_19.png') },
        { id: 9, src: require('../assets/images/1960698591-(1)_20.png') },

      ],



      loGo: [
        { id: 1, name: '三江学院', src: require('../assets/images/log.png') }
      ],


      naMe: [
        { id: 1, name: '三江学院', title: '一所伟大的学校,无论是闹鬼,老师死亡,学生遇难,校长被杀,都不能阻止他每年按时开学', src: require('../assets/images/banner.png'), logo: require('../assets/images/log.png') },
        { id: 2, name: '三江学院', title: '一所伟大的学校,无论是闹鬼,老师死亡,学生遇难,校长被杀,都不能阻止他每年按时开学', src: require('../assets/images/banner2.png'), logo: require('../assets/images/log.png') },
      
      ]











    }
  }
}

</script>




<style scoped>
.all {
  max-width: 414px;
  width: 100%;
  height: 100%;
  background-color: #f5f5f5;
  margin: 0 auto;
}

.nav {
  background-color: white;
  display: block;
  margin-bottom: 5%;
  padding-bottom: 5%;
}

.nav_1 {
  padding-top: 10px;
  padding-bottom: 10px;
}

.nav_1 p {
  font-size: 16px;
  padding-left: 10px;
  font-weight: 800;
}
.nav_1_in {
  display: flex;
  align-items: center;
}
.nav_1_in img {
  width: 40px;
  height: 40px;
  padding-left: 20px;
}
.tex {
  font-size: 16px;
  padding-left: 20px;
  padding-right: 20px;
  margin-top: 0px;
}

.im {
  max-width: 414px;
  width: 100%;
}
.im img {
  max-width: 375px;

  padding-right: 15px;
  padding-left: 20px;
}

.item3 {
  display: flex;
  justify-content: space-around;
  padding-left: 5%;
  padding-right: 5%;
  padding-bottom: 1%;
  flex-wrap: wrap;
}
.item3 img {
  width: 32%;
  height: 20%;
}

.foot {
  max-width: 414px;
  width: 100%;

  background-color: #0a0003;

  padding-top: 10px;
  padding-bottom: 10px;
  background-image: url("../assets/images/logo2.png");
  background-repeat: no-repeat;
  background-size: 50px;
  background-position: 5%;
}

.foot p {
  color: #ffffff;
  font-size: 14px;
  padding-left: 20%;
  font-weight: 800;
  margin: 0;
  display: inline;
}

.foot h2 {
  padding-left: 20%;
  margin: 0;
  color: #ffffff;
  display: inline;
  margin-right: 10%;
}

.foot a {
  color: #ffffff;
  border: 1px solid #ffdf08;
  border-radius: 15px;
  padding-left: 15px;
  padding-right: 15px;
  padding-top: 5px;
  padding-bottom: 5px;
  font-size: 16px;
  margin-right: 4%;
}

.footer {
  float: right;
  margin-top: 3%;
  margin-right: 5%;
}
</style>
