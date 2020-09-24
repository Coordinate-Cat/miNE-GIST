<script context="module">
	export function preload({ params, query }) {
		return this.fetch(`posts.json`).then(r => r.json()).then(posts => {
			return { posts };
		});
	}
</script>

<script>
	export let posts;
</script>

<style>
ul {
	margin: 1em 0 0 0;
	line-height: 1.5;
	padding-inline-start: 10px;
}

li{
	list-style: none;
	color: #fff;
	font-weight: bold;
}
</style>

<svelte:head>
	<title>Posts</title>
</svelte:head>

<h1>Recent posts</h1>

<ul>
	{#each posts as post}
		<!-- we're using the non-standard `rel=prefetch` attribute to
				tell Sapper to load the data for the page as soon as
				the user hovers over the link or taps it, instead of
				waiting for the 'click' event -->
		<li><a rel='prefetch' href='posts/{post.slug}'>{post.date}{post.title}</a></li>
	{/each}
</ul>