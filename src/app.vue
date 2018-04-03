<template>
	<div id='app'>
		<div id='cover'></div>
		<Header></Header>
		<List></List>
		<Footer></Footer>
	</div>
</template>

<script>
import Header from './webContent/header.vue';
import Footer from './webContent/footer.jsx';
import List from './webContent/todoList.vue';

export default{
	components:{
		Header,
		Footer,
		List,
	}
}
</script>

<style lang='stylus' scoped>
#app{
	#cover{
		background-color #999
		opacity 0.5
		z-index -1
	} 
}
</style>