<script>
	import Footer from './_component/Footer.svelte';
	import Header from './_component/Header.svelte';
</script>

<style>
    main {
        height: 100%;
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
				align-items: center;
        background-color: var(--bg-color);
    }
		.page-content{
				width : 100%;
        background-color: var(--bg-color);

		}

</style>

<main>
	<Header />

	<div class='page-content'>
		<slot />
	</div>

	<Footer />
</main>
