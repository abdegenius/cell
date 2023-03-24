<script>
    export let show = false;
</script>

<!-- Mobile menu, show/hide based on menu state. -->
<div class="{show ? 'block' : 'hidden'} border-b border-gray-700 md:hidden" id="mobile-menu">
	<div class="space-y-1 px-2 py-3 sm:px-3">
		<!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->
		<a
			href="#"
			class="bg-gray-900 text-white block rounded-md px-3 py-2 text-base font-medium"
			aria-current="page">Dashboard</a
		>

		<a
			href="#"
			class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium"
			>Team</a
		>

		<a
			href="#"
			class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium"
			>Projects</a
		>

		<a
			href="#"
			class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium"
			>Calendar</a
		>

		<a
			href="#"
			class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium"
			>Reports</a
		>
	</div>
	<div class="border-t border-gray-700 pt-4 pb-3">
		<div class="flex items-center px-5">
			<div class="flex-shrink-0">
				<img class="h-10 w-10 rounded-full" src="/user.png" alt="" />
			</div>
			<div class="ml-3">
				<div class="text-base font-medium leading-none text-white">John Doe</div>
				<div class="text-sm font-medium leading-none text-gray-400">john@doe.com</div>
			</div>
		</div>
		<div class="mt-3 space-y-1 px-2">
			<a
				href="#"
				class="block rounded-md px-3 py-2 text-base font-medium text-gray-400 hover:bg-gray-700 hover:text-white"
				>My Profile</a
			>

			<a
				href="#"
				class="block rounded-md px-3 py-2 text-base font-medium text-gray-400 hover:bg-gray-700 hover:text-white"
				>Settings</a
			>

			<a
				href="#"
				class="block rounded-md px-3 py-2 text-base font-medium text-gray-400 hover:bg-gray-700 hover:text-white"
				>Sign out</a
			>
		</div>
	</div>
</div>
