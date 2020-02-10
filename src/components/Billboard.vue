<template>
    <div id="Billboard">
        <div class="carousel-inner"><!--此处这个class不要动，是bootstrap写好的，删掉会使图中的字跑到下面去-->
            <img id="billboardImg" src="~@/assets/common/billboard.jpg" alt="Qianguan Billboard">
            <div class="container">
                <div class="carousel-caption">
                    <h1>{{title}}</h1>
                    <p>{{translation}}</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script type="text/javascript">
export default {
  data () {
    return {
      title: '西安前观测控技术有限公司',
      translation: 'Xi\'an Qianguan Measurement and Control Technology Co., LTD'
    }
  }
}

</script>

<style scoped>
#billboardImg {
    width: 100%;
}
.carousel-caption {
    text-shadow: #000000 5px 0 10px, #000000 0 5px 10px, #000000 -5px 0 10px, #000000 0 -5px 10px;
    margin-left: 0px;
}
</style>
