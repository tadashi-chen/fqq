<template>
	<div class="group-item" @click="click">
		<div class="avatar">
			<img :src="'/static/img/' + friendInfo.account + '.jpg'">
		</div>
		<div class="text">
			<p>{{ friendInfo.name }}</p>
			<span>[{{ friendInfo.state }}] {{ friendInfo.signature }}</span>
		</div>
	</div>
</template>

<script>
export default {
	props: ['friendInfo'],
	methods: {
		click () {
			this.fn.gotoConversation(this, this.friendInfo);
		}
	}
}
</script>

<style lang="scss" scoped>
	@import '../../assets/sass/function';
	.group-item {
		font-size: px2rem(44px);
		height: px2rem(180px);
		background-color: #fff;
		display: flex;
		border-bottom: 1px solid #e6e6e6;
		.avatar {
			display: flex;
			width: px2rem(204px);
			justify-content: center;
			align-items: center;
			> img {
				width: px2rem(132px);
				height: px2rem(132px);
				border-radius: 50%;
			}
		}
		.text {
			flex: 1;
			p {
				margin-top: px2rem(24px);
			}
			span {
				color: #808080;
				font-size: px2rem(38px);
			}
		}
	}
	.group-item:active {
		background-color: #f5f5f5;
	}
</style>