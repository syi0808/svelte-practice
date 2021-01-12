<script>
	import Hello from './Hello.svelte'
	import { storeName } from './store.js'

	let name

	const end = () => {
		$storeName = name;
	}
</script>

<input type="text" bind:value={name} />
<button on:click={end}>엔터</button>

<Hello />

<style>
</style>