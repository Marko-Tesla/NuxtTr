<template lang="pug">  
div.navbar
    nuxt-link(to="/")
      | Home
    nuxt-link(to="/about")
      | About 
    nuxt-link(to="/contact")
      | Contact 
</template>  
<style scoped>
	.navbar {
        display: flex;
		background: #0089a7;
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
		text-transform: uppercase;
        
	}

	.nuxt-link-exact-active {
		border-bottom: 2px solid black;
		padding-bottom: 8px;
	}
</style>