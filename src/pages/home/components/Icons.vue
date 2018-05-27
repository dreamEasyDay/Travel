<template>
	<div class="icons-wrapper">
		<div class="icon-content">
			<div class="icon-wrapper">
				<img src="http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png"/>
			</div>
			<p>图片</p>
		</div>
		<div class="icon-content">
			<div class="icon-wrapper">
				<img src="http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png"/>
			</div>
			<p>图片</p>
		</div><div class="icon-content">
			<div class="icon-wrapper">
				<img src="http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png"/>
			</div>
			<p>图片</p>
		</div>
		<div class="icon-content">
			<div class="icon-wrapper">
				<img src="http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png"/>
			</div>
			<p>图片</p>
		</div>
		<div class="icon-content">
			<div class="icon-wrapper">
				<img src="http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png"/>
			</div>
			<p>图片</p>
		</div>
		<div class="icon-content">
			<div class="icon-wrapper">
				<img src="http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png"/>
			</div>
			<p>图片</p>
		</div>
		<div class="icon-content">
			<div class="icon-wrapper">
				<img src="http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png"/>
			</div>
			<p>图片</p>
		</div>
		<div class="icon-content">
			<div class="icon-wrapper">
				<img src="http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png"/>
			</div>
			<p>图片</p>
		</div>
		<div class="icon-content">
			<div class="icon-wrapper">
				<img src="http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png"/>
			</div>
			<p>图片</p>
		</div>
	</div>
</template>

<script>
export default {
	name: 'HomeIcons'
}
</script>

<style lang="scss" scoped>
.icons-wrapper {
	width: 100%;
	height: 0;
	overflow: hidden;
	padding-bottom: 40%;
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
			text-align: center;
		}
	}
}
</style>