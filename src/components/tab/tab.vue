<template>
	<ul class="nav-list">
		
		<router-link tag="li" class="nav-item" to="/recommend">
			推荐
		</router-link>
		<router-link tag="li" class="nav-item" to="/singer">
			歌手
		</router-link>
		<router-link tag="li" class="nav-item" to="/rank">
			排行
		</router-link>
		<router-link tag="li" class="nav-item" to="/search">
			搜索
		</router-link>
	</ul>

</template>	
<script type="text/ecmascript-6">

</script>
<style scoped lang="scss" rel="stylesheet/scss">
@import "../../common/css/reset";

.nav-list{

	display:flex;
	.nav-item{
		flex:1;

	};
	.router-link-active{
		border:1px solid red
	}
}

</style>
