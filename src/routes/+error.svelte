<script lang="ts">
	import { page } from "$app/state";
</script>

<main class="min-h-screen flex items-center justify-center bg-gray-50 px-6">
	<div class="text-center">
		<h1 class="text-6xl font-bold text-primary-600 mb-4">Error {page.status}</h1>
		<p class="text-xl text-gray-600 mb-8">{page.error?.message ?? "Something went wrong."}</p>
		<a 
			href="/" 
			class="inline-block px-8 py-4 bg-primary-600 text-white font-semibold rounded-lg hover:bg-primary-700 transition-colors"
		>
			Go back home
		</a>
	</div>
</main>
