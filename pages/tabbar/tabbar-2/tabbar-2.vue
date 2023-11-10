<template>
	<view class="content">
		页面 - 2
		<view>
			<u-calendar :show="show"></u-calendar>
			<u-button @click="show = true">打开</u-button>
		</view>
	</view>
</template>

<script>
export default {
	data() {
		return {
			title: 'Hello',
			show: false
		};
	},
	onLoad() {},
	methods: {}
};
</script>

<style>
.content {
	text-align: center;
	height: 400upx;
	margin-top: 200upx;
}
</style>
