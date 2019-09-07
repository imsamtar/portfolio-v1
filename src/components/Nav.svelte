<script>
	export let segment;
</script>

<style>
	nav {
		z-index: 10;
		position: sticky;
		top: 0rem;
		height: 3rem;
		color: white;
		background: #000000cc;
		display: flex;
	}
	.logo {
		margin-left: 5rem;
		display: flex;
		align-items: center;
		text-decoration: none;
	}
	.menu {
		margin: 0 5rem 0 auto;
		list-style: none;
		display: flex;
		padding: 0;
	}
	.menu > li {
		width: 100%;
		display: flex;
		align-items: stretch;
		justify-content: space-evenly;
		margin: 0 0.1rem;
	}
	.menu > li:hover, .active { background: #00000077;}
	.menu > li > a {
		padding: 0.7rem;
		text-decoration: none;
	}
</style>

<nav>
	<a class="logo" href="/">
		<i class="fa fa-code"></i>
	</a>
	<ul class="menu">
		<li><a class:active={segment==undefined} href="/">Home</a></li>
		<li><a class:active={segment=='about'} href="/about">About</a></li>
		<li><a class:active={segment=='contact'} href="/contact">Contact</a></li>
		<li><a class:active={segment=='projects'} href="/projects">Projects</a></li>
		<li><a class:active={segment=='blog'} href="/blog">Blog</a></li>
	</ul>
</nav>