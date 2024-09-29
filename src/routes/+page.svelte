<script>
	import SvelteComponent1 from "../lib/components/SvelteComponent1.svelte";
	import SvelteComponent2 from "../lib/components/SvelteComponent2.svelte";
	import Button from "../lib/components/Button.svelte";

	let toggle = false;

	function handleClick() {
		toggle = !toggle
	}
</script>

<Button name={`${toggle ? 'Show Component 2' : 'Show Component 1'}`} on:toggle={handleClick}/>

{#if toggle}
	<div>
		<h1 class="text-center text-3xl font-bold">Component 1</h1>
		<SvelteComponent1 />
	</div>
{:else}
	<div>
		<h1 class="text-center text-3xl font-bold">Component 2</h1>
		<SvelteComponent2 />
	</div>
{/if}

