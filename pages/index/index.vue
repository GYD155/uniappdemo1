<template>
	<view class="content">
		<navigator url="/pages/list/list">跳转</navigator>
		<image class="logo" src="/static/logo.png"></image>
		
		<view class="text-area">
		<text class="title">{{title}}</text>	
	
		<scroll-view class="scroll" scroll-x>
			<view class="group">
			<view class="item">
				111
			</view >
			<view class="item">
				222
			</view>
			<view class="item">
				333
			</view>
			<view class="item">
				444
			</view>
			</view>
		</scroll-view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: '移动端'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="scss">
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
	.scroll{
		border:1px solid red;
		box-sizing: border-box;
		.group{
			white-space: nowrap;
			.item{
				width:220rpx;
				height:220rpx;
				background:royalblue;
				display: inline-block;
			}
		}
	}
</style>
