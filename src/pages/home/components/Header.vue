<template>
	<div class="header">
		<div class="header-left">
			<div class="iconfont back-icon">&#xe624</div>
		</div>
		<div class="header-input">
			<span class="iconfont">&#xe632</span>
			输入城市/景点/游玩主题
		</div>
		<div class="header-right">
			城市
			<span class="iconfont arrow-icon">&#xe64a</span>
		</div>
	</div>
</template>

<script>
export default {
	name: 'HomeHeader'
}
</script>

<style lang="scss" scored>
.header {
	display: flex;
	line-height: .86rem;
	background: #00bcd4;
	color: #fff;
	.header-left {
		float: left;
		display: block;
		width: .8rem;
		.back-icon {
			text-align: center;
			font-size: .4rem;
		}
	}
	.header-input {
		flex: 1;
		padding-left: 0.2rem;
		height: 0.64rem;
		line-height: .64rem;
		margin-top: .12rem;
		background: #fff;
		border-radius: 0.1rem;
		color: #ccc;
	}
	.header-right {
			width:1.24rem;
			float: right;
			text-align: center;
			.arrow-icon {
				font-size: .4rem;
				margin-left: -.04rem;
			}
		}
}
</style>