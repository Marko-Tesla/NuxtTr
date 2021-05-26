<template lang="pug">  
div.navbar
    nuxt-link(to="/")
      | home
    nuxt-link(to="/animations")
      | animations 
    nuxt-link(to="/about")
      | about 
</template>  
<style scoped>
	.navbar {
        display: flex;
		background: black;
		width: 100%;
		padding: 1rem;
		text-align: center;
		position: relative;
		z-index: 1000;
	}

	.navbar a {
		text-decoration: none;
		color: white;
		margin-right: 1rem;
        
	}

	.nuxt-link-exact-active {
		border-bottom: 2px solid white;
	}
</style>