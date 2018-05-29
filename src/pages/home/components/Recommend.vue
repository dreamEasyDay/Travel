<template>
	<div>
		<div class="recommend-title">热销推荐</div>
		<ul>
			<li class="item">
				<div class="item-img-wrapper">
					<img src="http://img1.qunarzz.com/sight/p0/1505/c0/c016dce7a3156fd1.water.jpg_200x200_9e096461.jpg"/>
				</div>
				<div class="item-info">
					<p class="item-title">福鼎太姥山</p>
					<p class="item-desc">福鼎太姥山甲天下，福鼎白茶，福鼎肉片，福鼎蜜汁鸡翅。</p>
					<a class="detail-link" href="#">查看详情</a>
				</div>
			</li>
		</ul>
	</div>	
</template>

<script>
export default {
	name: 'HomeRecommend'
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
			@include ellipsisSingleLine(78%);
			line-height: .54rem;
			font-size: .32rem;
		}
		.item-desc {
			@include ellipsisMultiLine(2, 78%);
			line-height: .4rem;
			color: #ccc;
		}
		.detail-link {
			
		}
	}
}
</style>