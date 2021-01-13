<script>
	import { storeName } from './store.js'
	import Router from 'svelte-spa-router'
	import routes from './routes'
	import { link } from 'svelte-spa-router'

	let name

	const end = () => {
		$storeName = name;
	}
</script>

<input type="text" bind:value={name} />
<button on:click={end}>엔터</button>
<a use:link href="/another">asd</a>

<Router {routes} />

<style>
</style>