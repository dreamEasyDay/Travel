<template>
	<div class="icons-wrapper">
		<swiper :options="swiperOption">
			<swiper-slide v-for="(page, index) of pages" :key="index">
				<div class="icon-content" v-for="item of page" :key="iconsList.id">
					<div class="icon-wrapper">
						<img :src="item.imgURL"/>
					</div>
					<p>{{item.desc}}</p>
				</div>
			</swiper-slide>
			<div class="swiper-pagination"  slot="pagination"></div>
		</swiper>
	</div>
</template>

<script>
export default {
	name: 'HomeIcons',
	data() {
		return {
			swiperOption: {
				pagination: '.swiper-pagination',
				loop: true
			},
			iconsList: [{
				id: '0001',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
				desc: '景点门桥'
			},{
				id: '0002',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/3e/86314b2af03b7502.png',
				desc: '一日游1'
			},{
				id: '0004',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
				desc: '景点门桥1'
			},{
				id: '0003',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/3e/86314b2af03b7502.png',
				desc: '一日游2'
			},{
				id: '0005',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
				desc: '景点门桥2'
			},{
				id: '0006',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/3e/86314b2af03b7502.png',
				desc: '一日游3'
			},{
				id: '0007',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
				desc: '景点门桥3'
			},{
				id: '0008',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/3e/86314b2af03b7502.png',
				desc: '一日游4'
			},{
				id: '0009',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
				desc: '景点门桥4'
			},{
				id: '0010',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/3e/86314b2af03b7502.png',
				desc: '一日游5'
			},{
				id: '0011',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
				desc: '景点门桥5'
			},{
				id: '0012',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/3e/86314b2af03b7502.png',
				desc: '一日游6'
			},{
				id: '0013',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
				desc: '景点门桥6'
			},{
				id: '0014',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/3e/86314b2af03b7502.png',
				desc: '一日游7'
			},{
				id: '0015',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
				desc: '景点门桥7'
			},{
				id: '0016',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/3e/86314b2af03b7502.png',
				desc: '一日游8'
			},{
				id: '0017',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
				desc: '景点门桥8'
			},{
				id: '0018',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/3e/86314b2af03b7502.png',
				desc: '一日游9'
			},{
				id: '0019',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
				desc: '景点门桥9'
			},{
				id: '0020',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/3e/86314b2af03b7502.png',
				desc: '一日游11'
			},{
				id: '0021',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
				desc: '景点门桥11'
			},{
				id: '0022',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/3e/86314b2af03b7502.png',
				desc: '一日游22'
			},{
				id: '0023',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
				desc: '景点门桥22'
			},{
				id: '0024',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/3e/86314b2af03b7502.png',
				desc: '一日游33'
			},{
				id: '0025',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
				desc: '景点门桥33'
			},{
				id: '0026',
				imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/3e/86314b2af03b7502.png',
				desc: '一日游44'
			}]
		}
	},
	computed: {
		pages () {
			const pages = []
			this.iconsList.forEach((item, index) => {
				const page = Math.floor(index/8)
				if(!pages[page]) {
					pages[page] = []
				}
				pages[page].push(item)
			})
			return pages;
		}
	}
}
</script>

<style lang="scss" scoped>
.icons-wrapper {
	width: 100%;
	height: 0;
	overflow: hidden;
	padding-bottom: 45%;
	.icon-content {
		float: left;
		width: 25%;
		padding-bottom: 20%;
		height: 0;
		overflow: hidden;
		.icon-wrapper {
			padding: 5% 20% 0;
			> img {
				width: 100%;
				display: block;
				margin: 0 auto;
				height: 100%;
			}
		}
		> p {
			padding: 0 .3rem;
			text-align: center;
			overflow: hidden;
			white-space: nowrap;
			text-overflow: ellipsis;
		}
	}
}
</style>