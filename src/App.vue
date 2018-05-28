<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style lang="scss">
.swiper-wrapper {
	.swiper-pagination-bullet-active {
		background: #fff !important;
	}
} 
.icons-wrapper {
	position: relative;
	.swiper-pagination-bullet-active {
		background: #00bcd4 !important;
	}
	.swiper-container {
		position: static;
	}
	.swiper-pagination {
		bottom: 0;
	}
}
.icons-wrapper .swiper-container {
	padding-bottom: 40%;
	height: 0;
}
</style>
