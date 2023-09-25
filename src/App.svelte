<script>
	import Main from './routes/Main.svelte';
	import Home from './routes/Home.svelte';
	import Project from './routes/Project.svelte';
	import Dashboard from './routes/Dashboard.svelte';
	import Header from './routes/Header.svelte';

	import Router from 'svelte-spa-router';

	const routes = {
		'/': Main,
		'/home': Home,
		'/project': Project,
		'/dashboard': Dashboard
	};
</script>

<main>
<Router {routes} />
</main>
