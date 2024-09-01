<script setup></script>

<template>
	<main>
		<article>
			<div class="inner">
				<div class="block glutter">
					<div class="container grid">
						<div class="start-1 cols-4 cols-m-8 start-m-1">some</div>
						<div
							class="scanline start-9 cols-8 start-m-1 cols-m-8"
							style="height: calc(460px + 10rem)"
						>
							<div class="scanline_wrapper">
								<div class="scanline_bg"></div>
								<svg
									xmlns="http://www.w3.org/2000/svg"
									class="icon icon_top_left"
									width="20"
									height="21"
									viewBox="0 0 20 21"
									fill="none"
									stroke="currentColor"
								>
									<path d="M10 0.332031V20.332"></path>
									<path d="M0 10.332L20 10.332"></path></svg
								><svg
									xmlns="http://www.w3.org/2000/svg"
									class="icon icon_bottom_left"
									width="20"
									height="21"
									viewBox="0 0 20 21"
									fill="none"
									stroke="currentColor"
								>
									<path d="M10 0.332031V20.332"></path>
									<path d="M0 10.332L20 10.332"></path>
								</svg>
								<svg
									xmlns="http://www.w3.org/2000/svg"
									class="icon icon_top_right"
									width="20"
									height="21"
									viewBox="0 0 20 21"
									fill="none"
									stroke="currentColor"
								>
									<path d="M10 0.332031V20.332"></path>
									<path d="M0 10.332L20 10.332"></path>
								</svg>
								<svg
									xmlns="http://www.w3.org/2000/svg"
									class="icon icon_bottom_right"
									width="20"
									height="21"
									viewBox="0 0 20 21"
									fill="none"
									stroke="currentColor"
								>
									<path d="M10 0.332031V20.332"></path>
									<path d="M0 10.332L20 10.332"></path>
								</svg>
							</div>
						</div>

						<div class="scanline-side">
							<div class="scanline_bg"></div>
							<div class="scanline_bg"></div>
						</div>
					</div>
				</div>
			</div>
		</article>
		<article>
			<div class="inner">
				<div class="block glutter">
					<div class="container grid">
						<div class="start-9 cols-8 start-m-1 cols-m-8">some</div>
						<div
							class="scanline start-1 cols-4 cols-m-8 start-m-1"
							style="height: calc(460px + 3rem)"
						>
							<div class="scanline_wrapper">
								<div class="scanline_bg"></div>
								<svg
									xmlns="http://www.w3.org/2000/svg"
									class="icon icon_top_left"
									width="20"
									height="21"
									viewBox="0 0 20 21"
									fill="none"
									stroke="currentColor"
								>
									<path d="M10 0.332031V20.332"></path>
									<path d="M0 10.332L20 10.332"></path></svg
								><svg
									xmlns="http://www.w3.org/2000/svg"
									class="icon icon_bottom_left"
									width="20"
									height="21"
									viewBox="0 0 20 21"
									fill="none"
									stroke="currentColor"
								>
									<path d="M10 0.332031V20.332"></path>
									<path d="M0 10.332L20 10.332"></path>
								</svg>
								<svg
									xmlns="http://www.w3.org/2000/svg"
									class="icon icon_top_right"
									width="20"
									height="21"
									viewBox="0 0 20 21"
									fill="none"
									stroke="currentColor"
								>
									<path d="M10 0.332031V20.332"></path>
									<path d="M0 10.332L20 10.332"></path>
								</svg>
								<svg
									xmlns="http://www.w3.org/2000/svg"
									class="icon icon_bottom_right"
									width="20"
									height="21"
									viewBox="0 0 20 21"
									fill="none"
									stroke="currentColor"
								>
									<path d="M10 0.332031V20.332"></path>
									<path d="M0 10.332L20 10.332"></path>
								</svg>
							</div>
						</div>
					</div>
				</div>
			</div>
		</article>
	</main>
	<div class="bg-grid-lines grid">
		<div class="line cols-4"></div>
		<div class="line cols-4"></div>
		<div class="line cols-4"></div>
		<div class="line cols-4"></div>
		<div class="line cols-4"></div>
	</div>
</template>

<style scoped>
main {
	display: flex;
	flex-direction: column;
	height: 100%;
}

article {
	position: relative;
	height: 100%;
	width: 100%;
}

article .inner {
	padding-top: 4rem;
	padding-bottom: 4rem;
}

.bg-grid-lines {
	position: fixed;
	top: 0;
	left: calc(var(--gutter-h));
	width: calc(100% - var(--gutter-h) * 2);
	height: 100%;
	box-sizing: border-box;
	pointer-events: none;
	-webkit-user-select: none;
	-moz-user-select: none;
	user-select: none;
	z-index: 2;
}

.bg-grid-lines .line {
	background: rgba(155, 155, 155, 0.2);
	width: 1px;
	height: 100%;
}

.bg-grid-lines .line:first-of-type {
	grid-area: 1 / 1 / 1 / 1;
}

.bg-grid-lines .line:nth-of-type(2) {
	grid-area: 1 / 5 / 1 / 9;
}

.bg-grid-lines .line:nth-of-type(3) {
	grid-area: 1 / 9 / 1 / 13;
}

.bg-grid-lines .line:nth-of-type(4) {
	grid-area: 1 / 13 / 1 / 17;
}

.bg-grid-lines .line:nth-of-type(5) {
	grid-area: 1 / 17 / 1 / 17;
}

.block {
	padding-top: 4rem;
	padding-bottom: 4rem;
	position: relative;
	height: 100%;
}

.scanline_wrapper {
	margin-right: calc(var(--gutter-h) * -1);
	width: calc(100% + var(--gutter-h) * 1);
}

.icon {
	position: absolute;
	width: 1rem;
	height: auto;
	opacity: 0.5;
	z-index: 1;
	color: #9a9a9a;
}

.icon.icon_bottom_left {
	bottom: -0.5rem;
	left: -0.5rem;
}

.icon.icon_top_left {
	top: -0.5rem;
	left: -0.5rem;
}

.icon.icon_top_right {
	top: -0.5rem;
	right: -0.5rem;
}

.icon.icon_bottom_right {
	bottom: -0.5rem;
	right: -0.5rem;
}

.scanline {
	position: relative;
	width: 100%;
	/*
	height: calc(460px + 10rem);
	*/
}

.scanline-side {
	display: flex;
	justify-content: space-between;
	position: absolute;
	top: 0;
	left: calc(var(--gutter-h) * -1);
	width: calc(100% + var(--gutter-h) * 2);
	height: 100%;
}

.scanline-side > .scanline_bg {
	position: relative;
	width: var(--gutter-h);
	display: block;
}

.scanline_bg {
	background: repeating-linear-gradient(
		-45deg,
		#000,
		#fff 2px,
		#fff 2px,
		#fff 6px
	);
	/*background-image: url(/scanline-dark.png);*/
	opacity: 0.08;
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
	pointer-events: none;
}

.glutter {
	left: calc(var(--gutter-h));
	width: calc(100% - var(--gutter-h) * 2);
}

.grid {
	display: grid;

	grid-template-columns: repeat(16, 1fr);
	grid-row-gap: 0;
	grid-column-gap: 0;
}

.gutter {
	padding-left: var(--gutter-h);
	padding-right: var(--gutter-h);
}

.container {
	position: relative;
	align-items: center;
	row-gap: 3rem;
}

@media (max-width: 1600px) {
	.grid {
		grid-template-columns: repeat(16, 1fr);
	}
}

@media (max-width: 1024px) {
	.grid {
		grid-template-columns: repeat(8, 1fr);
	}
}

@media (max-width: 768px) {
	.grid {
		grid-template-columns: repeat(8, 1fr);
	}
}

@media (max-width: 400px) {
	.grid {
		grid-template-columns: repeat(8, 1fr);
	}
}
</style>
