<script>
	import Heading from "./Heading.svelte";
	import Input from "./Input.svelte";
    import Text from "./Text.svelte";
    import Button from "./Button.svelte";
	import Image from "./Image.svelte";


</script>

<div class='flex flex-col w-[327px] mx-auto mt-16'>

<Image src='/image-comp2.png' type='component2'/>

<div class={`bg-[#202325] flex flex-col justify-center items-center px-6 pb-6 w-[327px] mx-auto rounded-b-2xl text-center font-["Inter"] `}>
    <Heading text='Introducing Virtual Reality'/>
    <Text text='Please check out all-new feature'/>
    <Input />
    <Button name='Sure' type='default' />
    <Button name='No, thanks' type='transparent' />
</div>

</div>