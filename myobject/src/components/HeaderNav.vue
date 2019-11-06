<template>
	<div class="box">
		<div class="left1">
			<ul class="left-ul">
				<li>
					<router-link class="nav" v-for="item in nvaLeft" :to="item.uri">{{item.name}}</router-link>
				</li>
			</ul>
		</div>
		<div class="right1">
			<ul class="right-ul">
				<li>
					<router-link class="nav" v-for="item in navRight" :to="item.uri">{{item.name}}</router-link>
				</li>
			</ul>
		</div>
	</div>
</template>

<script>
	export default {
		name: "HeaderNav",
		data() {
			return {
				nvaLeft: [{
					name: "翰墨书香",
					uri: "/"
				}, {
					name: "图书",
					uri: "/"
				}, {
					name: "小组",
					uri: "/"
				}, {
					name: "阅读",
					uri: "/"
				}, {
					name: "墨品",
					uri: "/"
				}, {
					name: "更多",
					uri: "/"
				}],
				navRight:[{
					name: "欢迎下载APP",
					uri: "/"
				},{
					name: "登录 / 注册",
					uri: "/"
				}]
			}
		}
	}
</script>

<style scoped="scoped">
	/* *{
		margin: 0;
		padding: 0;
	} */
	.box {
		height: 28px;
		width: 100%;
		background-color: #414141;
		position: relative;
	}

	.left1 {
		width: 660px;
		height: 28px;
		position: absolute;
		left: 20px;
	}

	.right1 {
		width: 220px;
		height: 28px;
		position: absolute;
		right: 20px;
	}

	.left-ul {
		list-style: none;
		font-size: 12px;
		color: #d5d5d5;
		float: left;
	}
	.nav {
		display: inline-block;
		height: 28px;
		width: 110px;
		text-decoration: none;
		font-size: 12px;
		color: #d5d5d5;
		line-height: 28px;
	}
</style>
