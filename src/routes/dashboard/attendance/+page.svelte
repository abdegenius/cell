<script>
	let history_modal = false;
</script>

<div class="relative mx-auto max-w-7xl px-4 pb-12 sm:px-6 lg:px-8">
	<div>
		<dl
			class="mt-4 flex flex-row items-stretch justify-start bg-white border border-gray-300 rounded-md shadow-md drop-shadow-md"
		>
			<div class="w-full bg-gray-50">
				<div class="relative overflow-x-auto scrollbar-hide max-h-[600px]">
					<table class="relative w-full text-sm text-left text-gray-500">
						<thead class=" w-full text-xs text-gray-700 uppercase bg-gray-50">
							<tr>
								<th scope="col" class="p-2"> Member </th>
								<th scope="col" class="p-2"> Date </th>
								<th scope="col" class="p-2"> Is Present </th>
								<th scope="col" class="p-2"> Action </th>
							</tr>
						</thead>
						<tbody class="pt-24 overflow-y-auto scrollbar-hide">
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="font-normal text-gray-900 whitespace-nowrap px-2">
									<div class="m-0 text-xs md:text-lg">John Doe</div>
								</th>
								<th scope="row" class="font-normal text-gray-900 whitespace-nowrap px-2">
									<div class="m-0 text-xs md:text-lg">24-03-2023</div>
								</th>
								<th scope="row">
									<button
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 font-medium rounded-lg text-sm p-2 text-center"
										type="button"
									>
										<i class="fa fa-check fa-1x" />
									</button>
									<button
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 font-medium rounded-lg text-sm px-3 py-2 text-center"
										type="button"
									>
										<i class="fa fa-times fa-1x" />
									</button>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (history_modal = true)}
										class="text-xs m-1 inline-flex text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm p-2 text-center "
										type="button"
									>
										HISTORY
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="font-normal text-gray-900 whitespace-nowrap px-2">
									<div class="m-0 text-xs md:text-lg">John Doe</div>
								</th>
								<th scope="row" class="font-normal text-gray-900 whitespace-nowrap px-2">
									<div class="m-0 text-xs md:text-lg">24-03-2023</div>
								</th>
								<th scope="row">
									<button
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 font-medium rounded-lg text-sm p-2 text-center"
										type="button"
									>
										<i class="fa fa-check fa-1x" />
									</button>
									<button
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 font-medium rounded-lg text-sm px-3 py-2 text-center"
										type="button"
									>
										<i class="fa fa-times fa-1x" />
									</button>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (history_modal = true)}
										class="text-xs m-1 inline-flex text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm p-2 text-center "
										type="button"
									>
										HISTORY
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="font-normal text-gray-900 whitespace-nowrap px-2">
									<div class="m-0 text-xs md:text-lg">John Doe</div>
								</th>
								<th scope="row" class="font-normal text-gray-900 whitespace-nowrap px-2">
									<div class="m-0 text-xs md:text-lg">24-03-2023</div>
								</th>
								<th scope="row">
									<button
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 font-medium rounded-lg text-sm p-2 text-center"
										type="button"
									>
										<i class="fa fa-check fa-1x" />
									</button>
									<button
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 font-medium rounded-lg text-sm px-3 py-2 text-center"
										type="button"
									>
										<i class="fa fa-times fa-1x" />
									</button>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (history_modal = true)}
										class="text-xs m-1 inline-flex text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm p-2 text-center "
										type="button"
									>
										HISTORY
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="font-normal text-gray-900 whitespace-nowrap px-2">
									<div class="m-0 text-xs md:text-lg">John Doe</div>
								</th>
								<th scope="row" class="font-normal text-gray-900 whitespace-nowrap px-2">
									<div class="m-0 text-xs md:text-lg">24-03-2023</div>
								</th>
								<th scope="row">
									<button
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 font-medium rounded-lg text-sm p-2 text-center"
										type="button"
									>
										<i class="fa fa-check fa-1x" />
									</button>
									<button
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 font-medium rounded-lg text-sm px-3 py-2 text-center"
										type="button"
									>
										<i class="fa fa-times fa-1x" />
									</button>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (history_modal = true)}
										class="text-xs m-1 inline-flex text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm p-2 text-center "
										type="button"
									>
										HISTORY
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="font-normal text-gray-900 whitespace-nowrap px-2">
									<div class="m-0 text-xs md:text-lg">John Doe</div>
								</th>
								<th scope="row" class="font-normal text-gray-900 whitespace-nowrap px-2">
									<div class="m-0 text-xs md:text-lg">24-03-2023</div>
								</th>
								<th scope="row">
									<button
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 font-medium rounded-lg text-sm p-2 text-center"
										type="button"
									>
										<i class="fa fa-check fa-1x" />
									</button>
									<button
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 font-medium rounded-lg text-sm px-3 py-2 text-center"
										type="button"
									>
										<i class="fa fa-times fa-1x" />
									</button>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (history_modal = true)}
										class="text-xs m-1 inline-flex text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm p-2 text-center "
										type="button"
									>
										HISTORY
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="font-normal text-gray-900 whitespace-nowrap px-2">
									<div class="m-0 text-xs md:text-lg">John Doe</div>
								</th>
								<th scope="row" class="font-normal text-gray-900 whitespace-nowrap px-2">
									<div class="m-0 text-xs md:text-lg">24-03-2023</div>
								</th>
								<th scope="row">
									<span class="text-green-600 font-bold text-xs text-center">PRESENT</span>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (history_modal = true)}
										class="text-xs m-1 inline-flex text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm p-2 text-center "
										type="button"
									>
										HISTORY
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="font-normal text-gray-900 whitespace-nowrap px-2">
									<div class="m-0 text-xs md:text-lg">John Doe</div>
								</th>
								<th scope="row" class="font-normal text-gray-900 whitespace-nowrap px-2">
									<div class="m-0 text-xs md:text-lg">24-03-2023</div>
								</th>
								<th scope="row">
									<span class="text-red-600 font-bold text-xs text-center">ABSENT</span>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (history_modal = true)}
										class="text-xs m-1 inline-flex text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm p-2 text-center "
										type="button"
									>
										HISTORY
									</button>
								</th>
							</tr>
						</tbody>
					</table>
				</div>
			</div>
		</dl>
	</div>
</div>


<div
	class="relative z-10 {history_modal ? 'block' : 'hidden'}"
	aria-labelledby="modal-title"
	role="dialog"
	aria-modal="true"
>
	<div class="fixed inset-0 bg-gray-500 bg-opacity-75 transition-opacity" />

	<div class="fixed inset-0 z-10 overflow-y-auto">
		<div class="flex min-h-full items-end justify-center p-4">
			<div
				class="relative transform overflow-hidden rounded-lg bg-white px-4 pt-5 pb-4 text-left shadow-xl transition-all sm:my-8 sm:w-full sm:max-w-lg sm:p-6"
			>
				<div class="mt-4">
					<ul class="flex justify-start flex-col space-y-2 divide-y divide-gray-300 overflow-y-auto scrollbar-hide">
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-green-600">PRESENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-red-600">ABSENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-green-600">PRESENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-red-600">ABSENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-green-600">PRESENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-red-600">ABSENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-green-600">PRESENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-red-600">ABSENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-green-600">PRESENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-red-600">ABSENT</small></span>
						</li><li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-green-600">PRESENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-red-600">ABSENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-green-600">PRESENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-red-600">ABSENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-green-600">PRESENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-red-600">ABSENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-green-600">PRESENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-red-600">ABSENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-green-600">PRESENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-red-600">ABSENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-green-600">PRESENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-red-600">ABSENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-green-600">PRESENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-red-600">ABSENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-green-600">PRESENT</small></span>
						</li>
						<li class="text-md font-medium text-gray-600 flex justify-between items-center space-x-6">
							<span>01-01-2023</span>
							<span><small class="text-red-600">ABSENT</small></span>
						</li>
					</ul>
				</div>

				<div class="mt-5">
					<button
						on:click={() => (history_modal = false)}
						type="button"
						class="mt-3 inline-flex w-full justify-center rounded-md bg-white px-3 py-2 text-sm font-semibold text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 hover:bg-gray-50 sm:ml-3 sm:mt-0 sm:w-auto"
						>Close</button
					>
				</div>
			</div>
		</div>
	</div>
</div>
