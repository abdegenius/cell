<script>
	import Header from '../../components/Header.svelte';
</script>

<div class="min-h-full">
	<div class="bg-gray-800 pb-32">
			<Header />
		<header class="py-10">
			<div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
				<h1 class="text-3xl font-bold tracking-tight text-white">Living Faith Home Cell | Barnawa</h1>
			</div>
		</header>
	</div>

	<main class="-mt-32">
		<slot></slot>
	</main>
</div>
