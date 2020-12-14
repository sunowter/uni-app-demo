<template>
	<view style="background:#F8F9FB">
		<view class="top-content">
			<image src="../../static/imgs/touxiang.jpg" mode="" class="avator"></image>
			<view class="name">YYT</view>
			<view class="text">你对讲师满意吗？</view>
			<view class="img-box">
				<image src="../../static/imgs/good.png" mode=""></image>
				<image src="../../static/imgs/bad.png" mode=""></image>
			</view>
		</view>
		<view class="bottom-content">
			<view class="" style="padding:40rpx 60rpx">
				<view class="">你对整个课程满意吗？</view>
				<view class="">
					<view class="" style="line-heigth:30px">
						<text>课程规划</text>
						<view class="rate"><uni-rate value="2" size="18"></uni-rate></view>
					</view>
					<view class="">
						<text>及时回复</text>
						<view class="rate"><uni-rate value="2" clsss="rate" size="18"></uni-rate></view>
					</view>
					<view class="">
						<text>及时回复</text>
						<view class="rate"><uni-rate value="2" clsss="rate" size="18"></uni-rate></view>
					</view>
				</view>
				<div>hahha </div>
				<input type="text" value="111" />
				<textarea class="advice" placeholder="你的反馈会督促我们做的更好" />
				<button type="primary" class="btn" @click="submitAdvice">提交评价</button>
				
			</view>
		</view>
	</view>
</template>

<script>
import uniRate from '@/components/uni-rate/uni-rate.vue';
export default {
	components: { uniRate },
	data() {
		return {};
	},
	created() {
		console.log('这个钩子会执行吗');
	},
	methods: {
		submitAdvice() {
			console.log('提价评价');
		}
	}
};
</script>

<style scoped lang="less">
.top-content {
	height: 394rpx;
	width: 100%;
	background: #fff;
	.avator {
		height: 80rpx;
		width: 80rpx;
		margin: 40rpx auto;
		display: block;
		/* border-radius:50%; */
	}
}

.name,
.text {
	text-align: center;
	line-height: 30px;
}
.img-box {
	width: 200rpx;
	margin: 20rpx auto;
}

.img-box image {
	height: 48rpx;
	width: 48rpx;
}
.img-box image:nth-child(1) {
	margin-right: 20px;
}
.bottom-content {
	margin-top: 20rpx;
	height: 794rpx;
	width: 100%;
	background: #fff;
	line-height: 70rpx;
}
.advice {
	width: 100%;
	height: 212rpx;
	margin: 40rpx auto;
	background: rgba(250, 250, 250, 1);
	border-radius: 12px;
	border: 2px solid rgba(213, 213, 213, 1);
}
.btn {
	margin: 40rpx auto 0;
	width: 100%;
	background: rgba(249, 111, 73, 1);
	color: white;
}
.rate {
	display: inline-block !important;
	margin-left: 20rpx;
}
</style>
