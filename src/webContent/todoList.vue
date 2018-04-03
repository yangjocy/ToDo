<template>
	<section class='todo'>
		<input 
		type="text"
		class="add-input item-font"
		placeholder="来添加新的任务吧" 
		autofocus="autofocus"
		@keyup.enter='addTodo' 
		>
		<item :todo='todo' class='item-font'></item>
	</section>
</template>

<script type="text/javascript">
import item from './item.vue';

export default {
	components:{
		item,
	},
	data(){
		return {
			todo:{
				id:0,
				content:'今天看完第二章',
				completed:false,
			}
		}
	},
	methods:{
		addTodo(){}
	}
}

</script>

<style lang='stylus' scoped>

.todo{
	margin 10px auto 10px auto
	width 90%
	border 1px solid gray
	box-shadow 1px 1px 5px white

	.add-input{
		width 100%
		border 1px solid
		padding 10px 10px 10px 60px	
	}
}
</style>