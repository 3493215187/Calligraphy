<template>
	<div class="footer">
		<div class="fnav public">
			<div class="logo">
				<p class="logo-p">翰墨书香 | 图书</p>
				<div class="logo-div">
					<p class="logo-p2">© 2019 market.douban.com, all rights reserved 翰墨书香股份有限公司</p>
					<p class="logo-p2">食品经营许可证: JY11105111524423</p>
					<p class="logo-p2">出版物经营许可证：新出发京批字第直170330号</p>
				</div>
			</div>
			<div class="right-logo">
				<ul class="right-l">
					<li>
						<router-link class="nav" v-for="item in nvaLeft" :to="item.uri">{{item.name}}</router-link>
					</li>
				</ul>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: "FooterNav",
		data() {
			return {
				nvaLeft: [{
					name: "购物说明",
					uri: "/"
				}, {
					name: "意见反馈",
					uri: "/"
				}, {
					name: "商务合作",
					uri: "/"
				}],
			}
		}
	}
</script>

<style scoped="scoped">
	.public {
		width: 1100px;
		margin: 0 auto;
	}

	.footer {
		height: 194px;
		width: 100%;
		background-color: #414141;
	}

	.fnav {
		height: 98px;
		padding-top: 50px;
		background-color: #01FF70;
	}

	.logo {
		display: inline-block;
		height: 98px;
		width: 397px;
		background-color: red;
		float: left;
	}

	.logo-p {
		height: 26px;
		background-color: green;
		color: #b5b5b5;
		font-size: 26px;
		text-align: left;
	}

	.logo-div {
		padding-top: 10px;
		height: 63px;
		background-color: gold;
	}

	.logo-p2 {
		height: 21px;
		color: #b5b5b5;
		font-size: 12px;
		text-align: left;
	}

	.right-logo {
		display: inline-block;
		height: 62px;
		width: 425px;
		background-color: #008000;
		float: right;
	}

	.right-l {
		float: left;
		list-style: none;
		text-align: center;
	}
	.nav{
		display: inline-block;
		height: 17px;
		width: 140px;
		color: #d5d5d5;
		font-size: 14px;
		text-decoration: none;
		padding-top: 10px;
		}
</style>
