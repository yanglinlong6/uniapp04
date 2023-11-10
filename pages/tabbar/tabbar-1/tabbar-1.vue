<template>
	<view class="content">
		页面 - 1
		<!-- <image class="logo" src="/static/logo.png"></image> -->
		<view class="text-area">
			<text class="title">{{ title }}</text>
			<u-button text="月落" @click="change(e)">nihao</u-button>
			<u-alert>nihao</u-alert>
			<text class="u-line-1">是日也，天朗气清，惠风和畅，仰观宇宙之大，俯察品类之盛</text>
		</view>
		<u-input placeholder="请输入内容" border="surround" v-model="value" @change="change"></u-input>
		
		<u-cell-group>
			<u-cell icon="setting-fill" title="个人设置"></u-cell>
			<u-cell icon="integral-fill" title="会员等级" value="新版本"></u-cell>
		</u-cell-group>
	</view>
</template>

<script>
import uAlert from '../../../uni_modules/uview-ui/components/u-alert/u-alert.vue';
export default {
	components: { uAlert },
	data() {
		return {
			title: 'Hello'
		};
	},
	onLoad() {},
	methods: {
		change(e) {
			console.log('change', e);
		}
	}
};
</script>

<style>
.content {
	text-align: center;
	height: 400upx;
	margin-top: 200upx;
}
</style>
