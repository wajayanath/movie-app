<template>
	<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
	  <router-link to="/" class="navbar-brand">Movie App</router-link>
	  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarColor02" aria-controls="navbarColor02" aria-expanded="false" aria-label="Toggle navigation">
	    <span class="navbar-toggler-icon"></span>
	  </button>
	  <div class="collapse navbar-collapse" id="navbarColor02">
	    <ul class="navbar-nav mr-auto">
	      <li class="nav-item active">
	      	<router-link to="/" class="nav-link"> Home </router-link>	
	      </li> 
<!-- 	      <li class="nav-item">
	        <a class="nav-link" href="#">Features</a>
	      </li>
	      <li class="nav-item">
	        <a class="nav-link" href="#">Pricing</a>
	      </li> -->
	      <li class="nav-item">
	        <router-link to="/about" class="nav-link"> About </router-link>
	      </li>
	    </ul>
	  </div>
	</nav>
</template>
<script>
	
</script>
<style>
	
</style>