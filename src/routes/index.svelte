<script>
	import Intro from '../components/Intro.svelte';
	import About from './about.svelte';
	import Projects from './projects.svelte';
	import Contact from './contact.svelte';
	import Footer from '../components/Footer.svelte';
</script>

<svelte:head>
	<title>My Portfolio</title>
</svelte:head>

<Intro />
<Projects />
<About />
<Contact />
<Footer />