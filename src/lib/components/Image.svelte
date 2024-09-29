<script>
    export let src = ''
    export let width = '120px'
    export let height = '120px'
    export let type='component1'
</script>


{#if type === 'component1'}
    <img class='rounded-2xl' src={src} alt='Main Image' width={width} height={height}/>
{/if}

{#if type === 'component2'}
    <img class='flex h-[186px] justify-center items-center self-stretch rounded-t-2xl' src={src} alt='Main Image'/>
{/if}