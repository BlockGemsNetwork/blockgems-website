<script lang="ts">
	export let id;
	export let caption;
	export let title;
	export let description;
	export let image;
	export let direction: 'left' | 'right' = 'left';

	let order = direction === 'left' ? ['content', 'image'] : ['image', 'content'];
</script>

<div {id} class="wide-section-wrapper no-bottom-padding">
	<div class="w-layout-grid wide-section-grid-halves">
		{#each order as o}
			{#if o === 'content'}
				<div class="wide-section-inner justify-contents-center bg-pastel-2 contents">
					<div class="container">
						<h6 class="subheading">{caption}</h6>
						<h2>{title}</h2>
						<div class="large-text">{description}</div>
						<!-- <div class="button-row">
                            <a href="#minter" class="button w-inline-block">
                                <div>Try Minter</div>
                            </a>
                        </div> -->
					</div>
				</div>
			{:else if o === 'image'}
				<div class="wide-section-inner screenshots">
					<div class="w-layout-grid screenshot-promo-grid">
						<img src={image} alt="" />
					</div>
				</div>
			{/if}
		{/each}
	</div>
</div>

<style lang="scss">
	.w-layout-grid {
		@media screen and (max-width: 991px) {
			.screenshots {
				order: 0;
			}

			.contents {
				order: 1;
			}
		}
	}
</style>
