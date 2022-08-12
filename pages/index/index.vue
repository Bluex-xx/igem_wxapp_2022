<template>
<view class="content">
	<image class="banner" src="../../static/banner.png"></image>
	<view class="select_content">
		<view class="select_menu">
			<image class="select_icon" style="width: 200rpx;height: 210rpx;" src="../../static/icon_1.png"></image>
			<view class="select_title">项目介绍</view>
		</view>
		<view class="select_menu">
			<image class="select_icon" src="../../static/icon_2.png"></image>
			<view class="select_title">血栓科普</view>
		</view>
		<view class="select_menu">
			<image class="select_icon" style="width: 180rpx;height: 180rpx;" src="../../static/icon_3.png"></image>
			<view class="select_title">关于我们</view>
		</view>
	</view>
	<view class="comment_content">
		<image src="../../static/comment_icon.png" class="comment_icon" style="left: 235rpx;"></image>
		<view class="comment_title">
			留言板
		</view>
		<image src="../../static/comment_icon.png" class="comment_icon" style="right: 235rpx;"></image>
		<view class="comment_input">
			<input v-model:value="value" placeholder="comment" placeholder-style="color:rgba(158, 158, 158, 0.46);font-weight:500;">
			<image src="../../static/comment_btn_icon.png" class="comment_btn"></image>
		</view>
		<view class="comment_list">
			
		</view>
	</view>
</view>
</template>

<script>
	export default {
		data() {
			return {
				value:''
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	.banner
	{
		width: 101%;
		margin-right: 1%;
	}
	.select_content
	{
		width: 100%;
		display: flex;
        justify-content: center;
		flex-wrap: nowrap;
	}
	.select_menu
	{
		width: 200rpx;
		height: 230rpx;
		margin: 30rpx 20rpx;
		position: relative;
		
	}
	.select_icon
	{
		width: 200rpx;
		height: 200rpx;
	}
	.select_title
	{
		position: absolute;
		bottom: 30rpx;
		left: 0;
		width: 100%;
		text-align: center;
		height: 20rpx;
	}
	.comment_content
	{
		width: 100%;
		position: relative;
	}
	.comment_title
	{
		font-size: 38rpx;
		text-align: center;
		margin-top: 30rpx;
	}
	.comment_icon
	{
		width: 50rpx;
		height: 50rpx;
		top: 30rpx;
		position: absolute;
	}
	.comment_input
	{
		margin:50rpx 193rpx;
		width: 300rpx;
		height: 50rpx;
		border: 1px solid #b6b6b6;
		border-radius: 10px;
		padding:10rpx 30rpx;
	}
	.comment_btn
	{
		width: 30rpx;
		height: 30rpx;
		position: absolute;
		right: 220rpx;
		top: 148rpx;
	}
	.comment_list
	{
		width: 90%;
		background: #f6f6f6;
		height: 300rpx;
		margin-left: 5%;
	}
</style>
