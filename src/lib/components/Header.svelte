<script>
	import RequestDemo from './RequestDemo.svelte';

	let y;
</script>

<div class="navbar-container">
	<div role="banner" class="navbar w-nav">
		<div class="navbar-row">
			<a href="/" aria-current="page" class="brand-link w-nav-brand w--current" aria-label="home">
				<img src="/blockgems-icon.svg" loading="eager" alt="" width="44" height="44" />
				<strong>BlockGems</strong>
			</a>
			<nav class="nav-menu w-nav-menu">
				<a href="/" aria-current="page" class="nav-link w-nav-link w--current">Home</a>
				<div data-hover="false" data-delay="200" class="nav-link w-dropdown">
					<div
						class="dropdown-toggle w-dropdown-toggle"
						id="w-dropdown-toggle-0"
						aria-controls="w-dropdown-list-0"
						aria-haspopup="menu"
						aria-expanded="false"
						role="button"
						tabindex="0"
					>
						<div>Products</div>
						<img
							src="/images/icon-chevron-down.svg"
							loading="eager"
							alt=""
							class="dropdown-toggle-icon"
						/>
					</div>
					<nav
						class="dropdown-list large-items w-dropdown-list"
						style="opacity: 0;"
						id="w-dropdown-list-0"
						aria-labelledby="w-dropdown-toggle-0"
					>
						<a href="/#minter" class="dropdown-link with-text w-inline-block" tabindex="0">
							<div class="dropdown-link-large-title">
								<div>Minter</div>
								<img src="/images/icon-arrow-up-right.svg" loading="eager" alt="" />
							</div>
						</a><a href="/#marketplace" class="dropdown-link with-text w-inline-block" tabindex="0">
							<div class="dropdown-link-large-title">
								<div>Marketplace</div>
								<img src="/images/icon-arrow-up-right.svg" loading="eager" alt="" />
							</div>
						</a><a href="/#spaces" class="dropdown-link with-text w-inline-block" tabindex="0">
							<div class="dropdown-link-large-title">
								<div>Spaces</div>
								<img src="/images/icon-arrow-up-right.svg" loading="eager" alt="" />
							</div>
						</a><a href="/#launchpad" class="dropdown-link with-text w-inline-block" tabindex="0">
							<div class="dropdown-link-large-title">
								<div>Launchpad</div>
								<img src="/images/icon-arrow-up-right.svg" loading="eager" alt="" />
							</div>
						</a>
					</nav>
				</div>
				<div class="dropdown-screen" style="opacity: 0;" />
				<a
					href="https://docsend.com/view/2hic5twtv3bib5bz"
					target="_blank"
					class="nav-link w-nav-link">Whitepaper</a
				>
			</nav>
			<div class="navbar-right-contents">
				<div class="navbar-button">
					<!-- <a href="https://blockgems.app" target="_blank" class="button small w-inline-block">
						<div class="small-text">Go to App</div>
						<img
							src="/images/icon-arrow-up-right-white.svg"
							loading="eager"
							alt=""
							class="arrow-link-icon"
						/>
					</a> -->

					<RequestDemo />
				</div>
				<div
					class="menu-button w-nav-button"
					style="-webkit-user-select: text;"
					aria-label="menu"
					role="button"
					tabindex="0"
					aria-controls="w-nav-overlay-0"
					aria-haspopup="menu"
					aria-expanded="false"
				>
					<img src="/images/icon-menu.svg" loading="eager" alt="" class="menu-button-icon" />
				</div>
			</div>
		</div>
		<div class="w-nav-overlay" data-wf-ignore="" id="w-nav-overlay-0" />
	</div>

	<div class="navbar-bg" class:visible={y >= 100} />
</div>

<svelte:window bind:scrollY={y} />

<style lang="scss">
	.brand-link {
		display: flex;
		align-items: center;

		img {
			width: 36px;
			height: 36px;
		}

		strong {
			font-family: 'Bespoke Serif', serif;
			font-size: 1.375rem;
			line-height: 1;
			margin-left: 1rem;

			position: relative;
			top: 1px;
		}
	}

	.nav-menu {
		flex: none;

		@media screen and (max-width: 991px) {
			display: none;
		}
	}

	.navbar-bg {
		opacity: 0;
		transition: all 0.3s;

		&.visible {
			opacity: 1;
		}
	}
</style>
