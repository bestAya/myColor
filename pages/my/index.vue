<template>
	<view>
		<view class="cu-list card-menu menu-avatar margin-top">
			<view class="cu-item">
				<view class="cu-avatar round lg" style="background-image:url(https://ossweb-img.qq.com/images/lol/img/champion/Taric.png);">
					<view class="cu-tag badge">99+</view>
				</view>
				<view class="content">
					<view class="text-grey">
						<view class="text-cut text-xl">瓦洛兰之盾-塔里克</view>
						<view class="cu-tag round bg-orange sm">战士</view>
					</view>
					<view class="text-gray text-sm flex">
						<view class="text-cut">
							塔里克是保护者星灵，用超乎寻常的力量守护着符文之地的生命、仁爱以及万物之美。塔里克由于渎职而被放逐，离开了祖国德玛西亚，前去攀登巨神峰寻找救赎，但他找到的却是来自星界的更高层的召唤。现在的塔里克与古代巨神族的神力相融合，以瓦洛兰之盾的身份，永不疲倦地警惕着阴险狡诈的虚空腐化之力。
						</view>
					</view>
				</view>
				<!-- <view class="action">
						<view class="text-grey text-xs">22:20</view>
						<view class="cuIcon-notice_forbid_fill text-gray"></view>
					</view> -->
			</view>
		</view>
		<view class="cu-list card-menu bg-white margin-top">
			<view class="cu-list menu sm-border">
				<view class="cu-item arrow">
					<view class="content">
						<text class="text-bold text-xl">我的订单</text>
					</view>
					<navigator hover-class="none" url="/pages/order/list" class="action">
						<text class="text-grey text-sm">查看更多</text>
					</navigator>
				</view>
			</view>
			<view class="cu-list grid col-4 no-border card-order">
				<view class="cu-item">
					<navigator hover-class="none" url="/pages/order/list?index=1">
						<view class="cuIcon-pay">
							<view class="cu-tag badge" v-if="item!=0">
								1
							</view>
						</view>
						<text>待付款</text>
					</navigator>
				</view>
				<view class="cu-item">
					<navigator hover-class="none" url="/pages/order/list?index=2">
						<view class="cuIcon-send">
							<view class="cu-tag badge" v-if="item!=0">
								1
							</view>
						</view>
						<text>待发货</text>
					</navigator>
				</view>
				<view class="cu-item">
					<navigator hover-class="none" url="/pages/order/list?index=3">
						<view class="cuIcon-deliver">
							<view class="cu-tag badge" v-if="item!=0">
								1
							</view>
						</view>
						<text>待收货</text>
					</navigator>
				</view>
				<view class="cu-item">
					<navigator hover-class="none" url="/pages/order/list?index=4">
						<view class="cuIcon-refund">
							<view class="cu-tag badge" v-if="item!=0">
								1
							</view>
						</view>
						<text>退货/售后</text>
					</navigator>
				</view>
			</view>
		</view>


		<view class="cu-list menu sm-border card-menu margin-top">
			<navigator hover-class="none" url="/pages/my/address" class="cu-item arrow">
				<view class="content">
					<text class="padding-right-sm text-xl iconfont icon-footprint text-bold"></text>
					<text class="">地址管理</text>
				</view>
			</navigator>
			<view class="cu-item arrow">
				<view class="content">
					<text class="padding-right-sm text-xl iconfont icon-like text-bold"></text>
					<text class="">我的收藏</text>
				</view>
			</view>
			<view class="cu-item arrow">
				<view class="content">
					<text class="padding-right-sm text-xl iconfont icon-time text-bold"></text>
					<text class="">浏览历史</text>
				</view>
			</view>
			<view class="cu-item arrow">
				<view class="content">
					<text class="padding-right-sm text-xl iconfont icon-like text-bold"></text>
					<text class="">在线客服</text>
				</view>
			</view>
			<view class="cu-item arrow">
				<view class="content">
					<text class="padding-right-sm text-xl iconfont icon-people text-bold"></text>
					<text class="">关于我们</text>
				</view>
			</view>
		</view>


	</view>
</template>
<script>
	export default {
		data() {
			return {
				result: [{

					photo: 'https://ossweb-img.qq.com/images/lol/web201310/skin/big81005.jpg',
					title: '韩版女式帽子',
					price: '600'
				}, {
					photo: 'https://ossweb-img.qq.com/images/lol/web201310/skin/big81005.jpg',
					title: 'shiahdiashdiashid',
					price: '600'
				}]
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>
<style>
	.card-order {
		padding: 0 !important;
		margin-top: 0 !important;
	}
</style>
