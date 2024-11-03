<template>
	<div class="video-container">
		<iframe
			class="responsive-iframe"
			width="560"
				height="315"
				src="https://www.youtube.com/embed/jm1TTSozPJM?si=ULFacT1hVfvfF3ZX"
				title="YouTube video player" frameborder="0"
				allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
				referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
	</div>
</template>

<script>
export default {
	name: 'VideoPlayer'
}
</script>
