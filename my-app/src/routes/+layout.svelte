<script>
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children()}

<style>    
    @font-face {
        font-family: 'Glory';
        src: url('$lib/assets/fonts/Glory-regular.ttf') format('truetype');
        font-weight: 400;
    }

    @font-face {
        font-family: 'Glory';
        src: url('$lib/assets/fonts/Glory-bold.ttf') format('truetype');
        font-weight: 700;
    }


    @font-face {
        font-family: 'LondrinaSolid';
        src: url('$lib/assets/fonts/LondrinaSolid-regular.ttf') format('truetype');
    }

</style>