<script>
	import { page } from '$app/stores';
</script>

<div class="flex w-full h-full items-center justify-center">
	<div
		class="w-auto h-auto sm:w-96 sm:h-96 bg-base-100 rounded-lg flex p-10 items-center justify-center transition-all duration-[0.25s] hover:scale-105 hover:bg-base-300 hover:shadow-2xl"
	>
		<div class="flex flex-col gap-10">
			<h1 class="text-4xl font-bold text-center">{$page.status}</h1>
			<p class="text-center font-semibold">{$page.error.message}</p>
		</div>
	</div>
</div>
