<script>
	import RequestDemo from '../RequestDemo.svelte';
</script>

<div class="section text-center wf-section">
	<div class="main-container">
		<div class="container-large align-center">
			<h1 class="display-heading">Creator economy ecosystem on Web3</h1>
			<div class="large-text">
				We aim to bridge DeFi and Crowdfunding with the digital Creator Economy.
			</div>
			<div class="button-row">
				<RequestDemo />
				<a href="#minter" class="button outline w-inline-block">
					<div>Learn More</div>
				</a>
			</div>
			<div class="link-below-contents justify-contents-center">
				<a href="https://docsend.com/view/2hic5twtv3bib5bz" target="_blank"
					>View our Whitepaper <img src="/images/icon-arrow-up-right.svg" alt="" /></a
				>
			</div>
		</div>
	</div>
</div>

<style lang="scss">
	.display-heading {
		line-height: 1.1;
	}

	.button-row {
		flex-direction: column;

		@media screen and (min-width: 768px) {
			justify-content: center;
			flex-direction: row;
		}

		a {
			margin-top: 1rem;

			@media screen and (min-width: 768px) {
				margin-left: 1rem;
				margin-top: 0;
			}

			&:first-child {
				margin-left: 0;
				margin-top: 0;
			}
		}
	}
</style>
