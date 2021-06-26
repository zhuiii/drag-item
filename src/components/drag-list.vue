<template>
<div>111s</div>
</template>

<script>
	export default {
		name: 'dragList',
		props: {
			list: {
				type: Array,
				default: () => ([])
			},
			itemHeight: {
				type: [Number],
				default: 70
			}
		}
	}
</script>

<style scoped>
	.drag-box {
		width: 100%;
		height: 100%;
		position: relative;

		
	}
	.drag-item {
		width: 100%;
		text-align: center;
		transition: all 0.5s;
		background-color: #fff;
		z-index: 1;
		border-bottom: 1rpx solid #F5F5F5;
		position: absolute;
	}

	.drag-active {
		box-shadow: 0 8px 20px 0 #e6e6e6;
		transform: scale(1.1);
		z-index: 9 !important;
		transition: box-shadow .5s, transform .5s, top 0s !important;
	}
</style>
