<script>
    import Image from "./Image.svelte";
    import Heading from "./Heading.svelte";
    import Text from "./Text.svelte";
    import Button from "./Button.svelte";

    export let width = 327;
    export let height = 420;
</script>

<div class={`bg-[#202325] flex flex-col justify-center items-center px-6 pt-8 pb-6 w-[${width}px] h-[${height}px] m-auto rounded-2xl text-center font-["Inter"] mt-24`}>
    <Image src={'/image-comp.png'} />
    <Heading />
    <Text />
    <Button name={'Sure'} type={'default'}/>
    <Button name={'No, thanks'} type={'transparent'}/>
</div>