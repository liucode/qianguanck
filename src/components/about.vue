<template>
    <div id="about">
        <div class="col-md-12">
            <div class="col-md-2"></div>
            <div class="col-md-8">
                <div class="row">
                    <h1>{{briefTitle}}</h1>
                </div>
                <div class="row">
                    <p class="lead" style="text-align: left;">{{briefIntro1}}</p>
                </div>
                <div class="row">
                    <p class="lead" style="text-align: left;">{{briefIntro2}}</p>
                </div>
                <hr>
            </div>
            <div class="col-md-2"></div>
        </div>
        <div class="col-md-12">
            <div class="col-md-2"></div>
            <div class="col-md-8">
                <div class="row">
                    <h1>{{achievementTitle}}</h1>
                </div>
                <div class="row">
                    <p class="lead" style="text-align: left;">{{achievementIntro}}</p>
                </div>
                <div class="row">
                    <div class="col-md-1"></div>
                    <div class="col-md-10">
                        <div class="col-md-4" v-for="picItem in picList1" :key="picItem"><img :src="picItem.pic" style="width: 100%;" /></div>
                    </div>
                    <div class="col-md-1"></div>
                </div>
                <hr>
            </div>
            <div class="col-md-2"></div>
        </div>
        <div class="col-md-12">
            <div class="col-md-2"></div>
            <div class="col-md-8">
                <div class="row">
                    <h1>{{envTitle}}</h1>
                </div>
                <div class="row">
                    <p class="lead" style="text-align: left;">{{envIntro}}</p>
                </div>
                <div class="row">
                    <div class="col-md-1"></div>
                    <div class="col-md-10">
                        <div class="col-md-4" v-for="picItem in picList2" :key="picItem"><img :src="picItem.pic" style="width: 100%;" /></div>
                    </div>
                    <div class="col-md-1"></div>
                </div>
            </div>
            <div class="col-md-2"></div>
        </div>
        <p>&nbsp;</p>
    </div>
</template>

<script type="text/javascript">
export default {
  data () {
    return {
      briefTitle: '公司简介',
      briefIntro1: '西安前观测控技术有限公司，成立于2017年3月8日。公司主要从事“超大规模应力实时检测系统”、“高速基因比对设备”等科研工作和产业化应用实践。公司由具有多年科研开发工作经验的精干技术人员组成。',
      briefIntro2: '公司现有员工8人，直接从事产品开发的6人。上述人员中，正高级工程师1人，工程师6人， 助理工程师1人，开发人员平均年龄33岁。',
      achievementTitle: '公司成果及资质',
      achievementIntro: '经过2年多的发展，公司已取得许多相关技术的认证，并获得了多项发明专利以及软件著作权等各类资质认证，此外，主要项目的校准认证也已经完成并获得了校准证书。',
      envTitle: '公司环境',
      envIntro: '公司位于西北地区核心城市陕西省西安市，办公地点位于西安市碑林环大学创新产业带-西安创新设计中心大楼。园区内智力人才密集，科技成果汇聚，具备浓厚的创新创业氛围。附近还有西安交通大学、西北工业大学、西安电子科技大学等一流高校，人才储备丰富。',
      picList1: [{
        pic: require('../assets/about/calibration1.jpg')
      },
      {
        pic: require('../assets/about/calibration1.jpg')
      },
      {
        pic: require('../assets/about/calibration1.jpg')
      },
      {
        pic: require('../assets/about/calibration1.jpg')
      },
      {
        pic: require('../assets/about/calibration1.jpg')
      },
      {
        pic: require('../assets/about/calibration1.jpg')
      }],
      picList2: [{
        pic: require('../assets/about/env1.jpg')
      },
      {
        pic: require('../assets/about/env2.jpg')
      },
      {
        pic: require('../assets/about/env3.jpg')
      }]
    }
  }
}
</script>

<style scoped="true">
    img {
        transition: all 0.8s;
    }
    img:hover {
        transform: scale(1.7);
        position: sticky;
        z-index: 10;
    }
</style>
