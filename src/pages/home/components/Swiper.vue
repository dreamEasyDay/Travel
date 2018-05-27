<template>
	<div class="swiper-wrapper">
		<swiper :options="swiperOption">
			<!-- slides -->
			<swiper-slide v-for="item of swiperList" :key="item.id">
				<img class="swiper-img" :src="item.imgURL"/>
			</swiper-slide>
			<!-- Optional controls -->
			<div class="swiper-pagination"  slot="pagination"></div>
		</swiper>
	</div>
</template>

<script>
export default {
	name: 'HomeSwiper',
	data() {
		return{
			swiperOption: {
				pagination: '.swiper-pagination',
				loop: true
			},
			swiperList: [{
				id: '0001',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1805/cb/2110021e0365b702.jpg_750x200_05a70d80.jpg'
			}, {
				id: '0002',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1805/22/b25372f55c6eef02.jpg_750x200_89dc3964.jpg'
			}]
		}
	}
}
</script>

<style lang="scss" scoped>
.swiper-wrapper >>> .swiper-pagination-bullet-active {
	background: #fff !important;
}
.swiper-wrapper {
	width: 100%;
	height: auto;
	.swiper-img {
		width: 100%;
	}
}
</style>