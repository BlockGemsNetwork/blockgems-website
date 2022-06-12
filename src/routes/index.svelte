<script>
	import IndexClients from '$lib/components/index/IndexClients.svelte';
	import IndexHero from '$lib/components/index/IndexHero.svelte';
	import IndexProductBlock from '$lib/components/index/IndexProductBlock.svelte';
	import RequestDemo from '$lib/components/RequestDemo.svelte';
</script>

<div style="opacity: 1;" class="load-first">
	<IndexHero />
</div>

<div style="opacity: 1;" class="load-second">
	<IndexProductBlock
		id="minter"
		image="/images/product-graphic-1.png"
		caption="with Minter"
		title="Content Tokenisation"
		description="Allows content creators to upload a digital copy of their art or content, and create a Non Fungible Token in whole or in fractions."
	/>

	<IndexProductBlock
		id="marketplace"
		image="/images/product-graphic-2.png"
		caption="with Marketplace"
		title="Content Marketplace"
		description="A curated hub for content creators to list their work for sale or auction."
		direction="right"
	/>

	<IndexProductBlock
		id="spaces"
		image="/images/product-graphic-3.png"
		caption="with Spaces"
		title="Content Subscription"
		description="A self-curated and self-managed member area for all content creators."
	/>

	<IndexProductBlock
		id="launchpad"
		image="/images/product-graphic-4.png"
		caption="with Launchpad"
		title="Content Crowdfunding"
		description="Allows content creators to crowdfund in exchange for early / special access."
		direction="right"
	/>

	<!-- <div class="section wf-section">
		<div class="main-container">
			<div class="section-title">
				<div class="container increased-width align-center">
					<h3 class="text-center">Grow quickly with a robust suite of features.</h3>
				</div>
			</div>
			<div class="w-layout-grid grid-halves">
				<div class="container increased-width">
					<div
						class="fade-in-on-scroll---first"
						style="opacity: 1; transform: translate3d(0px, 0px, 0px) scale3d(1, 1, 1) rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg); transform-style: preserve-3d;"
					>
						<div class="graphic-box bg-pastel-2">
							<img
								src="https://assets.website-files.com/6201f3e1c045ec64c27060a2/620ae0203b478200ea179545_graphic-icon-01.png"
								loading="lazy"
								alt=""
								class="graphic-box-image"
								width="290"
							/>
						</div>
						<h4 class="heading-below-image">Understand Your Audience</h4>
						<div>
							Pellentesque erat id amet vel proin aliquam diam. Et non quis tellus elementum nulla
							quam curabitur.
						</div>
						<div class="link-below-contents reduced-margin">
							<a href="https://medium.com/@blockgemsorg" target="_blank">Explore Blog</a>
						</div>
					</div>
				</div>
				<div class="container increased-width">
					<div
						class="fade-in-on-scroll---second"
						style="opacity: 1; transform: translate3d(0px, 0px, 0px) scale3d(1, 1, 1) rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg); transform-style: preserve-3d;"
					>
						<div class="graphic-box bg-pastel-3">
							<img
								src="https://assets.website-files.com/6201f3e1c045ec64c27060a2/620ae021d3816d469b6a9dd8_graphic-icon-02.png"
								loading="lazy"
								alt=""
								class="graphic-box-image"
								width="290"
							/>
						</div>
						<h4 class="heading-below-image">Grow Customers</h4>
						<div>
							Enim nec auctor in etiam scelerisque. Egestas tristique euismod eget gravida nisl. A
							egestas orci egestas dapibus faucibus.
						</div>
						<div class="link-below-contents reduced-margin">
							<a href="/template/style-guide">View Usecases</a>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>

	<IndexClients /> -->

	<div class="section wf-section">
		<div class="main-container">
			<h6 class="subheading">We empower creators from all walks of life</h6>
			<div class="w-layout-grid headings-grid">
				<div>
					<div class="large-heading no-bottom-margin">Content Creators</div>
				</div>
				<div>
					<div class="large-heading no-bottom-margin">Play-to-Earn Games</div>
				</div>
				<div>
					<div class="large-heading no-bottom-margin">NFT Projects</div>
				</div>
				<div>
					<div class="large-heading no-bottom-margin">Influencers</div>
				</div>
				<div>
					<div class="large-heading no-bottom-margin">Global Brands</div>
				</div>
			</div>
			<div class="button-row">
				<RequestDemo />
			</div>
		</div>
	</div>
</div>
