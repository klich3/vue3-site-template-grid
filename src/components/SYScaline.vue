<template>
	<div class="scanline">
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
</template>

<style scoped>
.scanline {
	position: relative;
	width: 100%;
	min-height: 460px;
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
	color: var(--scaline-cross-color, #9a9a9a);
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
</style>
