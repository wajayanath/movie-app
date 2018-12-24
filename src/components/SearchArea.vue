<template>
	<div class="form-group row">
			      <label for="inputMail" class="col-lg-2">Search Movie</label>
			      <div class="col-lg-6">
			      	<input type="text" class="form-control" id="inputMail" placeholder="Type here" @input="keyPressed">
			      </div>
	</div>
</template>
<script>
	import axios from 'axios'
	export default {
		data () { 
			return {
				newSet:[]
			}
		},
		methods: {
			 keyPressed(event) {
			 	var key = event.target.value;
			 	axios.get("https://yts.am/api/v2/list_movies.json?query_term="+ key)
			 		.then(response=>{
			 			this.newSet = response.data.data.movies;
			 		})
			 		.catch(e=>{
			 			this.error.push(e)
			 		});
			this.$emit('newDataset',this.newSet);  

			 }
		}
	}
	
</script>
<style>
</style>