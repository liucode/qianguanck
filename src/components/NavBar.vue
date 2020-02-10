<template>
    <div id="NavBar">
        <div class="container">
            <div><img :src="logoTop" style="height: 50px;" /></div>
            <div v-for="tagItem in navBar" :key="tagItem"><router-link :to="tagItem.url">{{tagItem.tag}}</router-link></div>
        </div>
    </div>
</template>

<script type="text/javascript">
export default {
  data () {
    return {
      logoTop: require('../assets/common/logo_top.jpg'),
      navBar: [{
        url: '/',
        tag: '首      页'
      },
      {
        url: '/about',
        tag: '公司介绍'
      },
      {
        url: '/products',
        tag: '产品中心'
      }]
    }
  }
}

</script>

<style>
    #NavBar {
        height: 51px;
    }
    .container {
        float: left;
    }
    .container > div {
        display: inline;
        text-decoration: none;
        font-size: 18px;
        font-weight: 800;
        margin-left: 40px;
        white-space: pre-wrap;
    }
    a:link {
        color: #686868;
		text-decoration: none;
    }
    a:visited {
        color: #686868;
        text-decoration: none;
		text-underline-color: #FF0000;
		border-bottom: 5px solid #FF0000;
    }
    a:hover {
        color: #E0E0E0;
        text-decoration: none;
    }
</style>
