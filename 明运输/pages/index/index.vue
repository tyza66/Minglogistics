<template>
	<view>
		<view class="top"></view>
		<image class="title" src="../../static/tags/title.png"></image>
		<view class="icons">
			<view class="oneicon">
				<image src="../../static/icons/a1.png"></image>
				<p>查询货物</p>
			</view>
			<view class="oneicon">
				<image src="../../static/icons/a2.png"></image>
				<p>ETC</p>
			</view>
			<view class="oneicon">
				<image src="../../static/icons/a3.png"></image>
				<p>信息大全</p>
			</view>
			<view class="oneicon">
				<image src="../../static/icons/a4.png"></image>
				<p>保险</p>
			</view>
			<view class="oneicon">
				<image src="../../static/icons/a5.png"></image>
				<p>签约车队</p>
			</view>
			<view class="oneicon">
				<image src="../../static/icons/a6.png"></image>
				<p>运输管家</p>
			</view>
			<view class="oneicon">
				<image src="../../static/icons/a7.png"></image>
				<p>时讯</p>
			</view>
			<view class="oneicon">
				<image src="../../static/icons/a8.png"></image>
				<p>账户金融</p>
			</view>
		</view>
		<view class="ye">
			<image src="../../static/icons/qb.png"></image>
			<view>
				<p>运费金额</p>
				<p>9600元</p>
			</view>
			<view>
				<p>打款时间</p>
				<p>3月8日</p>
			</view>
			<view>
				<p>账户余额</p>
				<p>53996元</p>
			</view>
		</view>
		<image class="info" src="../../static/tags/info.png" @click="gn()"></image>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {
			gn(){
				console.log("123")
				uni.navigateTo({
					url:"/pages/index/gn/gn"
				});
			}
		}
	}
</script>

<style>
	.top {
		height: var(--status-bar-height);
		width: 100%;
		background-color: #FFFFFF;
	}

	.title {
		width: 100%;
		height: 160rpx;
	}

	.icons {
		width: 100%;
		height: 370rpx;
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;	
	}
	
	.oneicon{
		width: 170rpx;
		height: 170rpx;
		margin: 0 auto;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}
	.oneicon image{
		width: 100rpx;
		height: 100rpx;
	}
	.oneicon p{
		margin-top: 5rpx;
	}
	.ye{
		width: 100%;
		height: 130rpx;
		background: #fdf79f;
		border-radius: 45rpx;
		display: flex;
		flex-direction: row;
		justify-content: left;
		align-items: center;
	}
	.ye image{
		width: 70px;
		height: 100rpx;
		margin-left: 25rpx;
	}
	.ye view{
		display: flex;
		flex-direction: column;
		justify-content: left;
		align-items: center;
		margin-left: 30rpx;
	}
	.info{
		width: 100%;
		height: 555rpx;
		flex-direction: row;
		justify-content: center;
		align-items: center;
	}
</style>
