<template>
	<div class="item">
		<input 
		type="checkbox" 
		v-model='todo.completed'
		>
		<label class="light-font">{{todo.content}}</label>
		<button 
		class="delBtn" 
		@click='delTodo'
		></button>
	</div>
</template>


<script type="text/javascript">
export default {
	props:{
		todo:{
			type: Object,
			required:true,
		}
	},
	methods:{
		delTodo(){

		}
	}

}
</script>

<style lang='stylus'>
.delBtn{
float right
}
</style>