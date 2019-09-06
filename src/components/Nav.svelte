<script>
	export let segment;
</script>

<style>
	nav {
		height: 3rem;
		color: white;
		background: #00000088;
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
	.menu > li:hover { background: #00000077;}
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
		<li><a href="/">Home</a></li>
		<li><a href="#about">About</a></li>
		<li><a href="#contact">Contact</a></li>
		<li><a href="#project">Projects</a></li>
		<li><a href="#blog">Blog</a></li>
	</ul>
</nav>