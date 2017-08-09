<template>
	
	<ul>
		
	</ul>
</template>	
<script type="text/ecmascript-6">
	import {getDiscList} from '../../api/recommend' 
	import {ERR_OK} from '../../api/config'
	export default {
		data(){
			return{
				discList: []
			}
			 			
		},
		created(){
		  this._getDiscList()
		},
		methods :{

			_getDiscList(){
				 getDiscList().then((res) => {
		          if (res.code === ERR_OK) {
		            this.discList = res.data.list
		            console.log(this.discList)
		          }
		        })
			}
		}
	}
</script>
<style type="text/css">
 	
</style>