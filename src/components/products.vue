<template>
	<div id="products">
		<h1 style="font-weight: bold;">{{pageTitle}}</h1>
		<div class="col-md-12">
			<div class="col-md-2"></div>
			<div class="col-md-8">
				<div class="row">
					<h2>{{productInfo[0].pTitle}}</h2>
				</div>
				<div class="row">
					<p>{{productInfo[0].pProfile}}</p>
				</div>
				<div class="row">
					<img class="col-md-12" :src="productInfo[0].pPic" />
				</div>
				<div class="row">
					<video id="pVideo" class="video-js vjs-big-play-centered vjs-fluid">
						<source :src="productInfo[1].pVideo" type="video/mp4"></source>
					</video>
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
			pageTitle: '产品中心',
			productInfo: [{
				pTitle: '西安航空学院静力试验平台',
				pProfile: '我司于2019年下半年为西安航空学院提供一套航空部件静力试验教学平台。',
				pPic: require('../assets/products/product1/pic1.jpg'),
				// pVideo: require('../assets/products/product2/acquisitionUnit.mp4')
			},
			{
				pTitle: '现场采集单元',
				pProfile: '现场采集单元',
				// pPic: require('../assets/products/product1/pic1.jpg'),
				pVideo: require('../assets/products/product2/acquisitionUnit.mp4')
			}
			]
		}
	},
	mounted() {
		this.initVideo();
	},
	methods: {
		initVideo() {
			let myPlayer = this.$video(pVideo, {
				controls: true,
				autoplay: 'play',
				preload: "auto",
				// width: "1200px",
				// height: "720px",
			});
		}
	}
}
</script>

<style>
</style>
