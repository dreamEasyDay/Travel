<template>
	<div>
		<div class="recommend-title">热销推荐</div>
		<ul>
			<li class="item" v-for="item of itemsList" :key="item.id">
				<div class="item-img-wrapper">
					<img :src="item.imgURL"/>
				</div>
				<div class="item-info border-bottom">
					<p class="item-title">{{item.title}}</p>
					<p class="item-desc">{{item.desc}}</p>
					<a class="detail-link" :href="item.btnLink">查看详情</a>
				</div>
			</li>
		</ul>
	</div>	
</template>

<script>
export default {
	name: 'HomeRecommend',
	data () {
		return {
			itemsList: [{
				id: '0001',
				imgURL: 'http://img1.qunarzz.com/sight/p0/1505/c0/c016dce7a3156fd1.water.jpg_200x200_9e096461.jpg',
				title: '福鼎太姥山1',
				desc: '福鼎太姥山甲天下，福鼎白茶，福鼎肉片，福鼎蜜汁鸡翅',
				btnLink: 'https://www.imooc.com/u/6663422/szcourses/list'
			},{
				id: '0002',
				imgURL: 'http://img1.qunarzz.com/sight/p0/1505/c0/c016dce7a3156fd1.water.jpg_200x200_9e096461.jpg',
				title: '福鼎太姥山2',
				desc: '福鼎太姥山甲天下，福鼎白茶，福鼎肉片，福鼎蜜汁鸡翅',
				btnLink: 'www.baidu.com'
			},{
				id: '0003',
				imgURL: 'http://img1.qunarzz.com/sight/p0/1505/c0/c016dce7a3156fd1.water.jpg_200x200_9e096461.jpg',
				title: '福鼎太姥山3',
				desc: '福鼎太姥山甲天下，福鼎白茶，福鼎肉片，福鼎蜜汁鸡翅',
				btnLink: 'www.baidu.com'
			},{
				id: '0004',
				imgURL: 'http://img1.qunarzz.com/sight/p0/1505/c0/c016dce7a3156fd1.water.jpg_200x200_9e096461.jpg',
				title: '福鼎太姥山4',
				desc: '福鼎太姥山甲天下，福鼎白茶，福鼎肉片，福鼎蜜汁鸡翅',
				btnLink: 'www.baidu.com'
			}]
		}
	}
}
</script>

<style lang="scss" scoped>
.recommend-title {
	margin-top: .2rem;
	padding: 0 .28rem;
	line-height: .8rem;
	background: #eee;
}
.item {
	overflow: hidden;
	display: flex;
	height: 1.9rem;
	.item-img-wrapper {
		> img {
			width: 1.7rem;
			height: 1.7rem;
			padding: .1rem;

		}
	}
	.item-info {
		flex: 1;
		padding: .1rem;
		.item-title {
			@include ellipsisSingleLine(60%);
			line-height: .54rem;
			font-size: .32rem;
		}
		.item-desc {
			@include ellipsisSingleLine(85%);
			line-height: .6rem;
			color: #ccc;
		}
		.detail-link {
			margin-top: .2rem;
			padding: .08rem .2rem;
			line-height: .6rem;
			background: #ff9300;
			color: #fff;
			border-radius: .12rem;
		}
	}
}
</style>