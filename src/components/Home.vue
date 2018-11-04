<template>
	<div>
		Home组件--{{this.$store.state.count}}
		
		<button @click="incCount()">增加</button>
	</div>
</template>

<script>
	import store from '../vuex/store.js'
	
	export default{
		data(){
			return{
				msg:'我是home组件'
			}
		},
		store,
		methods:{
			incCount(){
				 this.$store.commit('incCount');
			}
		}
	}
</script>

<style>
</style>