<script>
	export let segment;
	import logo from '../../static/logo.png';

	function gotoHome() {
		window.location.href = ".";
	}
</script>

<style>
	nav {
		border-bottom: 1px solid rgba(255,62,0,0.1);
		font-weight: 300;
		padding: 0 1em;
		position: sticky;
		top: 0;
		width: 100%;
		z-index: 100;
		background-color: mistyrose;
	}

	ul {
		margin: 0;
		padding: 0;
	}

	ul::after {
		content: '';
		display: block;
		clear: both;
	}

	li {
		display: block;
		float: left;
		transition: all 400ms;
	}

	li:hover {
		color: crimson;
	}

	[aria-current] {
		position: relative;
		display: inline-block;
	}

	[aria-current]::after {
		position: absolute;
		content: '';
		width: calc(100% - 1em);
		height: 2px;
		background-color: rgb(255,62,0);
		display: block;
		bottom: -1px;
	}

	a {
		text-decoration: none;
		padding: 1em 0.5em;
		display: block;
	}

	#logo {
		height: 48px;
		padding-right: 16px;
		padding-top: 4px;
		padding-left: 6px;
	}

	#logo:hover {
		cursor: pointer;
	}
</style>

<nav>
	<ul>
		<li><img alt="logo" src="{logo}" on:click="{gotoHome}" id="logo"></li>
		<li><a aria-current="{segment === undefined ? 'page' : undefined}" href=".">Home</a></li>
		<li><a aria-current="{segment === 'about' ? 'page' : undefined}" href="about">About</a></li>

		<!-- for the blog link, we're using rel=prefetch so that Sapper prefetches
		     the blog data when we hover over the link or tap it on a touchscreen -->
		<li><a rel=prefetch aria-current="{segment === 'blog' ? 'page' : undefined}" href="blog">Blog</a></li>
		<li><a aria-current="{segment === 'test' ? 'page' : undefined}" href="test">Test</a></li>
	</ul>
</nav>
