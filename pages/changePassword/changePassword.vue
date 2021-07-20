<template>
	<view class="content">
		<image src="../../static/background.png"></image>
		<view class="gradient-ltor">
			<view class="gradient-utod">
				<image class="logo" src="../../static/logo.png"></image>
				<view class="formmodul">
					<form action="">
						<view class="worknum">
							<van-field
							    class="field"
								label=""
							    left-icon="../../static/account.png"
							    placeholder="工号"
								placeholder-class="phstyle"
							/>
							<!-- <image style="width: 28rpx;height: 30rpx;" src="../../static/account.png" mode=""></image> -->
							<!-- <input type="text" placeholder="工号" placeholder-class="phstyle"> -->
							<van-field
								class="field"
							    label=""
							    left-icon="../../static/phone.png"
							    placeholder="原密码"
								placeholder-class="phstyle"
							/>
							<van-field
							    class="field"
								label=""
							    left-icon="../../static/password.png"
							    placeholder="请输入密码"
								placeholder-class="phstyle"
							/>
							<switch></switch>
							<van-field
							    class="field"
								label=""
							    left-icon="../../static/password.png"
							    placeholder="再次输入密码"
								placeholder-class="phstyle"
							/>
							<switch></switch>
						</view>
						<button type="default">保存</button>
						<!-- <view class="">
							<image style="width: 24rpx;height: 30rpx;" src="../../static/phone.png" mode=""></image>
							<input type="text" placeholder="原密码" placeholder-class="phstyle">
						</view>
						<view class="">
							<image style="width: 23rpx;height: 30rpx;" src="../../static/password.png" mode=""></image>
							<input type="password" placeholder="请输入密码" placeholder-class="phstyle">
							<switch></switch> -->
							<!--  :checked="areaPosterSwitch" -->
						<!-- </view>
						<view class="">
							<image style="width: 23rpx;height: 30rpx;" src="../../static/password.png" mode=""></image>
							<input style="border: none;" type="password" placeholder="再次输入密码" placeholder-class="phstyle">
							<switch></switch>
						</view> -->
					</form>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	import field from '../../component/vant/lib/field/index';
	export default {
		data() {
			return {
				text: '333',
				title: 'Hello',
				value1: 'zdzs'
			}
		},
		onLoad() {

		},
		methods: {
		
		},
		components: {
		    "van-field": field,
		},
	}
</script>

<style scoped>
	.content {
		width: 100%;
		height: 100%;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	
	.content>image{
		width: 100%;
		height: 100%;
		position: absolute;
	}

	.logo {
		height: 192rpx;
		width: 192rpx;
		border-radius: 192rpx;
		margin: auto auto;
		padding-top: 52rpx;
		display: flex;
		z-index: 1;
	}
	
	.formmodul{
		height: 728rpx;
		width: 624rpx;
		display: flex;
		background-color: white;
		margin: -90rpx auto auto auto;
		border-radius: 20rpx;
		-moz-box-shadow:0 0 10rpx #ddd;
		-webkit-box-shadow:0 0 10rpx #ddd;
		box-shadow:0 0 10rpx #ddd;
		position: relative;
	}

	.formmodul input{
		height: 120rpx;
		width: 550rpx;
		line-height: 120rpx;
		border-bottom: 1rpx solid lightgray;
		margin-left: 7%;
	}

	.formmodul image{
		position: absolute;
		left: 50rpx;
		margin-top: 45rpx;
	}

	button::after{ 
		border: none;
	} 

	.formmodul button{
		width: 528rpx;
		height: 80rpx;
		line-height: 80rpx;
		background-color: #2f8739;
		margin-top: 30rpx;
		border: none;
		outline: none;
		font-size: 36rpx;
		color: white;
		border-radius: 40rpx;
		margin-left: 48rpx;
	}

	.formmodul switch{
		transform: scale(0.7,0.7);
		position: absolute;
		right: 10%;
		margin-top: -12%;
	}

	.worknum{
		margin-top: 100rpx;
		margin-left: 47rpx;
	}
	
	.worknum .field{
		font-size: 28rpx;
		width: 530rpx;
		height: 120rpx;
		line-height: 120rpx;
		padding-left: 46rpx;
	}
	
	.worknum >>> van-field{
		font-size: 28rpx;
	}
	
	.phstyle{
		font-size: 28rpx;
		margin-left: 80rpx;
	}
	
	/* .gradient-ltor{
		width: 100%;
		height: 350rpx;
		background: -webkit-linear-gradient(to right, rgb(176,236,204), rgb(226,246,208) rgb(185,218,251));
		background: -o-linear-gradient(to right, rgb(176,236,204), rgb(185,218,251));
		background: -moz-linear-gradient(to right, rgb(176,236,204), rgb(185,218,251));
		background: linear-gradient(to right, rgb(176,236,204), rgb(185,218,251));
	}
	
	.gradient-utod{
		width: 100%;
		height: 100%;
		background: -webkit-linear-gradient(rgba(188,239,207,0.4), #fff);
		background: -o-linear-gradient(rgba(188,239,207,0.4), #fff);
		background: -moz-linear-gradient(rgba(188,239,207,0.4), #fff);
		background: linear-gradient(rgba(188,239,207,0.4), #fff);
	} */
</style>
