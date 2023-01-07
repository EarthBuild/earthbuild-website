<script>
	// Import the Mobile Detector
	import { isMobile } from '$lib/isMobile.svelte';

	// Load the stylesheet
	import '../app.css';

	function copyLink() {
		navigator.clipboard.writeText('earthbuild.de');
	}	
</script>

<div>
	<!-- svelte-ignore a11y-click-events-have-key-events -->
	{#if !isMobile}
	 <div class="card_left" on:click={copyLink}>
			<div style="font-size: 24px;font-weight:700;left:7%;position:relative;">EARTHBUILD.DE</div>
			<div style="font-size: 14px;font-weight:700;color:blue;position:absolute;top:63%;left:7%;">
			Klicke zum kopieren
		</div>
	</div>
	{/if}
	<div class="logo">
		<a href="https://earthbuild.de/">
			<img alt="Earthbuild Logo" src="/logo.webp" />
		</a>
	</div>
	<a href="https://discord.gg/fmxNNE3xnH">
		<div class="card_right">
			<div style="font-size: 24px;font-weight:700;left:7%;position:relative;">DISCORD</div>
			<div style="font-size: 14px;font-weight:700;color:blue;position:absolute;top:63%;left:7%;">
				Klicke zum joinen
			</div>
		</div>
	</a>
</div>
