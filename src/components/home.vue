<template>
    <div id="home">
        <div class="row"  v-for="introItem in introList" :key="introItem">
            <div class="col-md-12" id="rowInfoForHome">
                <div class="col-md-6" id="pic">
                    <img :src="introItem.pic1" style="width: 100%;">
                </div>
                <div class="col-md-6" id="text" style="padding: 8%;">
                    <h2 class="featurette-heading">{{introItem.title1}}</h2>
                    <p class="lead">{{introItem.content1}}</p>
                </div>
            </div>
            <div class="col-md-12" id="rowInfoForHome">
                <div class="col-md-6" id="text" style="padding: 8%;">
                    <h2 class="featurette-heading">{{introItem.title2}}</h2>
                    <p class="lead">{{introItem.content2}}</p>
                </div>
                <div class="col-md-6"  id="pic">
                    <img :src="introItem.pic2" style="width: 100%;">
                </div>
            </div>
        </div>
        <p>&nbsp;</p>
    </div>
</template>

<script type="text/javascript">
export default {
  data () {
    return {
      introList: [{
        title1: '飞机强度试验',
        content1: '解决飞机强度试验中信号线缆多、信号标定难、测量精度差、缺乏实时性等问题，同时提高实验可信度、提高实验效率，并可节约试验经费。',
        pic1: require('../assets/home/pic1.jpg'),
        title2: '舰船应变监测',
        content2: '解决舰船航行安全问题，如：触礁、暗流、遇袭、船体结构疲劳等，可及时反馈并报警，及时处置和损管。',
        pic2: require('../assets/home/pic2.jpg')
      },
      {
        title1: '矿井安全监测',
        content1: '矿井冲击地压预警，实时监测矿道结构强度，一旦矿井结构出现异常，可为人员撤离提供时间窗口，有力保障井下施工安全。',
        pic1: require('../assets/home/pic3.jpg'),
        title2: '路桥静载试验',
        content2: '预防公路、桥梁的过载，预警路桥坍塌危害，有效保障出行人员的生命及财产安全。',
        pic2: require('../assets/home/pic4.jpg')
      }]
    }
  }
}

</script>

<style scoped="true">
    #text {
        padding: 8%;
    }
    #pic {
        padding: 3%;
    }
    #rowInfoForHome:hover {
        background-color: #E3E3E3;
    }
</style>
