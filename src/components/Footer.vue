<template>
    <div id="Footer">
        <hr>
        <div class="col-md-12">
            <div class="col-md-8" id="title">
                <div class="col-md-2"></div>
                <div class="col-md-6">
                    <h3>Contact us</h3>
                </div>
            </div>
        </div>
        <div class="col-md-12">
            <div class="col-md-8">
                <div class="col-md-2"></div>
                <div class="col-md-6">
                    <table>
                    <tr>
                        <td>{{mail}}</td>
                        <td class="tbinfo">{{mailInfo}}</td>
                    </tr>
                    <tr>
                        <td>{{tel}}</td>
                        <td class="tbinfo">{{telInfo}}</td>
                    </tr>
                    <tr>
                        <td>{{addr}}</td>
                        <td class="tbinfo">{{addrInfo}}</td>
                    </tr>
                </table>
                </div>
            </div>
        </div>
        <div class="col-md-12">
            <div class="col-md-8">
                <div class="col-md-2"></div>
                <div class="col-md-6">
                    <p style="text-align: left; white-space: pre-wrap;">&copy;{{cpright}}</p>
                </div>
            </div>
            <p><a href="#" style="color: #D0D0D0;">Back to top ↑</a></p>
        </div>
    </div>
</template>

<script type="text/javascript">
export default {
  data () {
    return {
      mail: '邮箱：',
      mailInfo: 'service@xaqgck.com',
      tel: '电话：',
      telInfo: '12312312345',
      addr: '地址：',
      addrInfo: '陕西省西安市碑林区二环南路西段69号',
      cpright: ' 2019 Xi\'an Qianguan Measurement and control Co., Ltd'
    }
  }
}

</script>

<style>
    #Footer {}
    .tbinfo {
        text-align: left;
    }
    .pull-right {
        margin-right: 15%;
    }
    #title {
        text-align: left;
    }
    h3 {
        margin-top: 0.05%;
    }
</style>
