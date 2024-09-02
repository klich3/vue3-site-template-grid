<template>
	<div class="bg-grid-lines grid">
		<div class="line cols-4"></div>
		<div class="line cols-4"></div>
		<div class="line cols-4"></div>
		<div class="line cols-4"></div>
		<div class="line cols-4"></div>
	</div>
</template>

<style scoped>
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
	background: var(--scaline-color);
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
</style>
