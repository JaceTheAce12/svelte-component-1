<script>
	import SvelteComponent1 from "../lib/components/SvelteComponent1.svelte";
	import SvelteComponent2 from "../lib/components/SvelteComponent2.svelte";
	import Button from "../lib/components/Button.svelte";

	let showComponent2 = false;

	const toggle = () => {
		showComponent2 = !showComponent2;
	}
</script>

<Button name={`${showComponent2 ? 'Show Component 2' : 'Show Component 1'}`} on:click={toggle}/>

{#if showComponent2}
	<SvelteComponent1 />
{:else}
	<SvelteComponent2 />
{/if}

