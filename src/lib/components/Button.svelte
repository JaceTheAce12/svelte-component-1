<script>
    import { createEventDispatcher } from "svelte";

    export let name = '';
    export let type = 'default';
    export let color = '';
    export let width = 279;

    const dispatch = createEventDispatcher();

    function handleClick() {
        dispatch('toggle');
    }
</script>


{#if type === 'default'}
    <button on:click={handleClick} class={`flex w-[279px] h-[48px] p-[16px] justify-center items-center rounded-[48px] bg-[#6B4EFF] mt-6 hover:bg-[#5538EE] ease-in-out duration-300`}>{name}</button>
{/if}

{#if type === 'transparent'}
    <button on:click={handleClick} class={`flex w-[279px] h-[48px] p-[16px] justify-center items-center rounded-[48px] mt-3 hover:bg-[#C6C4FF] hover:text-[#6B4EFF] ease-in-out duration-300`}>{name}</button>
{/if}

