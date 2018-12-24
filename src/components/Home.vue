<template>
	<div class="container">
		<div>
			<form>
			  <fieldset>
			    <legend>Movie App</legend>
			    <app-search @newDataset="results = $event"></app-search>
			  </fieldset>
			</form>
		</div>
		<div class="row">
			 <div class="col-lg-12">
			 	<app-result :resList="results"></app-result>
			 	<!-- {{ results }} -->
			 </div>
		</div>
	</div>
	
</template>
<script>

import SearchArea from './SearchArea.vue'
import ResultArea from './ResultArea.vue'

export default {
	data() {
		return {
			results:[]
		}
	},
	components: {
	'app-search' : SearchArea,
	'app-result' : ResultArea
	}
}

</script>
<style>
	
</style>