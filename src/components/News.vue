<template>
	<div>
		<div>
		news组件--{{this.$store.state.count}}
		
		<button @click="incCount()">增加</button>
	</div>
	</div>
</template>

<script>
	import store from '../vuex/store.js'
	
	export default{
		data(){
			return{
				msg:'新闻组件'
			}
		},
		store,
		methods:{
			incCount(){
				this.$store.commit('incCount')
			}
		}
		
	}
</script>

<style>
</style>