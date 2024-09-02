<template>
	<div class="scanline-side">
		<div class="scanline_bg"></div>
		<div class="scanline_bg"></div>
	</div>
</template>

<style scoped>
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
</style>
