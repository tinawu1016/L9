<template>
 <article class="card">
	<img :src="movie.Poster" :alt="movie.Title">
	 <h2>{{ movie.Title }}</h2>
	 <!--<p class="card__copy">{{ movie.Year }}</p>-->
 </article>
</template>

<script>
export default {
	props: {
		movie: Object
	}
}
</script>


<style>
.card {
	margin: 1rem;
	border: 1px solid #000;
	padding: 1.5rem;
	max-width: 200px;
	min-height: 200px;
}
</style>
