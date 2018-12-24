<template>
      <div>
 <!--      	{{ resList }} -->
      	<div v-for="item in resList">
      		<div class="row">
    	      	<div class="col-lg-3">
		          <a href="#">
		            <img class="img-fluid rounded mb-3 mb-md-0" :src="item.medium_cover_image" alt="">
		          </a>
		        </div>
		        <div class="col-lg-9">
		          <h3>{{ item.title }} - {{ item.year }}</h3>
		          <h5>IMDB Rating - {{ item.rating }}   {{ item.genres }}</h5>
		          <hr>
		          <p>{{ item.summary }}</p>
		          <a class="btn btn-primary" :href="item.url" target="_blank">show more</a>
		        </div>
		    </div>
		        <br/>
         </div>
      </div>
</template>
<script>
	export default {
		props: ['resList']  
	}
</script>
<style>
	
</style>