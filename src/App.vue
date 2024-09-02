<script setup></script>

<template>
	<main>
		<article>
			<div class="inner">
				<div class="block gutter">
					<div class="container grid">
						<div class="start-1 cols-4 cols-m-8 start-m-1">some</div>

						<SYScaline
							class="start-9 cols-8 start-m-1 cols-m-8"
							style="height: calc(460px + 10rem)"
						/>

						<SYScalineSide />
					</div>
				</div>
			</div>
		</article>
		<article>
			<div class="inner">
				<div class="block gutter">
					<div class="container grid">
						<div class="start-9 cols-8 start-m-1 cols-m-8">some</div>
						<SYScaline
							class="start-1 cols-4 cols-m-8 start-m-1"
							style="height: calc(460px + 3rem)"
						/>
					</div>
				</div>
			</div>
		</article>

		<SYScalineBg />
	</main>
</template>

<script setup>
import SYScaline from "@/components/SYScaline.vue";
import SYScalineSide from "@/components/SYScaline-side.vue";
import SYScalineBg from "@/components/SYScaline-bg.vue";
</script>

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

.block {
	padding-top: 4rem;
	padding-bottom: 4rem;
	position: relative;
	height: 100%;
}

.block > .container {
	position: relative;
	align-items: center;
	row-gap: 3rem;
}

.gutter {
	left: calc(var(--gutter-h));
	width: calc(100% - var(--gutter-h) * 2);
}
</style>
