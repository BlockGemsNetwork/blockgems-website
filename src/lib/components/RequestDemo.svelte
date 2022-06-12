<script lang="ts">
	const requestDemo = () => {
		(window as any).Calendly.initPopupWidget({
			url: 'https://calendly.com/blockgems/request-demo'
		});
		return false;
	};
</script>

<svelte:head>
	<link href="https://assets.calendly.com/assets/external/widget.css" rel="stylesheet" />
	<script
		src="https://assets.calendly.com/assets/external/widget.js"
		type="text/javascript"
		async></script>
</svelte:head>

<a href={'#'} on:click={requestDemo} class="button w-inline-block">
	Request Demo
	<img src="/images/icon-arrow-up-right-white.svg" loading="lazy" alt="" class="button-icon" />
</a>
