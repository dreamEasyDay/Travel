<template>
	<div>
		<div class="recommend-title">周末去哪儿</div>
		<ul>
			<li class="item" v-for="item of itemsList" :key="item.id">
				<div class="item-img-wrapper">
					<img :src="item.imgURL"/>
				</div>
				<div class="item-info border-bottom">
					<p class="item-title">{{item.title}}</p>
					<p class="item-desc">{{item.desc}}</p>
				</div>
			</li>
		</ul>
	</div>	
</template>

<script>
export default {
	name: 'HomeWeekend',
	data () {
		return {
			itemsList: [{
				id: '0001',
				imgURL: 'http://img1.qunarzz.com/sight/source/1711/15/1cdd5ee885686b.jpg_r_640x214_46768064.jpg',
				title: '小白浪',
				desc: '小各种嗨皮各种浪，不一样的水上漂流。',
			},{
				id: '0002',
				imgURL: 'http://img1.qunarzz.com/sight/source/1711/15/1cdd5ee885686b.jpg_r_640x214_46768064.jpg',
				title: '小白浪2',
				desc: '小各种嗨皮各种浪，不一样的水上漂流。',
			},{
				id: '0003',
				imgURL: 'http://img1.qunarzz.com/sight/source/1711/15/1cdd5ee885686b.jpg_r_640x214_46768064.jpg',
				title: '小白浪',
				desc: '小各种嗨皮各种浪，不一样的水上漂流。',
			},{
				id: '0004',
				imgURL: 'http://img1.qunarzz.com/sight/source/1711/15/1cdd5ee885686b.jpg_r_640x214_46768064.jpg',
				title: '小白浪',
				desc: '小各种嗨皮各种浪，不一样的水上漂流。',
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
	display: block;
	.item-img-wrapper {
		width: 100%;
		> img {
			width: 100%;
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
	}
}
</style>