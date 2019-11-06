<template>
	<div>
		<!-- 顶部导航栏 -->
		<header-nav></header-nav>
		
		<!-- 中间部分 -->
		<router-view></router-view>
		
		<!-- 底部导航栏 -->
		<footer-nav></footer-nav>
	</div>
</template>

<script>
	import HeaderNav from "./HeaderNav"
	import FooterNav from "./FooterNav"
	export default {
		name: "Home",
		data() {
			return {}
		},
		components:{
			"header-nav": HeaderNav,
			"footer-nav": FooterNav
		}
	}
</script>

<style>

</style>
