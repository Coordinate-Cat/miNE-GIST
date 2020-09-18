<script>
	export let segment;
</script>

<style>
	nav {
		position: fixed;
    right: 0;
    left: 0;
    z-index: 999;
		margin-bottom: 0;
		background-color: #bbb;
		font-size: 18px;
	}

	ul {
		margin: 0 0 0 20px ;
		padding: 0;
	}

	/* clearfix */
	ul::after {
		content: '';
		display: block;
		clear: both;
	}

	li {
		display: block;
		float: left;
	}

	[aria-current] {
		position: relative;
		display: inline-block;
	}

	[aria-current]::after {
		position: absolute;
		content: '';
		left: 0;
		width: 100%;
		height: 3px;
		background-color: rgb(255,62,0);
		display: block;
		bottom: -3px;
	}

	a {
		text-decoration: none;
		padding: 0 10px;
		display: block;
		color: #000;
		background-color: #bbb;
	}

	a:hover {
		color: #bbb;
		background-color: #000;
	}
</style>

<nav>
	<ul>
		<li><a aria-current="{segment === undefined ? 'page' : undefined}" href=".">home</a></li>
		<li><a aria-current="{segment === 'about' ? 'page' : undefined}" href="about">about</a></li>

		<!-- for the blog link, we're using rel=prefetch so that Sapper prefetches
		the blog data when we hover over the link or tap it on a touchscreen -->
		<li><a rel=prefetch aria-current="{segment === 'blog' ? 'page' : undefined}" href="blog">scaffolding</a></li>
		<li><a href="https://github.com/Coordinate-Cat">Github</a></li>
	</ul>
</nav>
