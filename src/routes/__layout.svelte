<script>
	import Footer from '$lib/components/Footer.svelte';
	import Header from '$lib/components/Header.svelte';
	import LoadingContainer from '$lib/components/LoadingContainer.svelte';
	import BackToTop from '$lib/components/BackToTop.svelte';
</script>

<Header />

<slot />

<LoadingContainer />

<Footer />
