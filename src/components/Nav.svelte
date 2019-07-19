<style>
    nav {
        display: grid;
        grid-template-columns: max-content auto max-content;
    }
    .logo {
        display: grid;
        grid-auto-flow: column;
        place-content: center;
        padding: 0 20px;
        text-transform: uppercase;
        font-size: 1.6rem;
        font-weight: 300;
        height: 70px;
    }
    .main-menu {
        display: grid;
        grid-auto-flow: column;
        grid-gap: 10px;
        list-style: none;
        align-items: center;
        padding: 0 20px;
    }
    a {
        text-decoration: none;
        font-weight: 500;
    }
</style>
<nav>
    <a href="/" alt="Logo" class="logo">Sameer Tariq</a>
    <div class="space">.</div>
    <ul class="main-menu">
        <li class="main link"><a href="/">Home</a></li>
        <li class="main link"><a href="/projects">Projects</a></li>
        <li class="main link"><a href="/skills">Skills</a></li>
        <li class="main link"><a href="/contact">Contact</a></li>
    </ul>
</nav>