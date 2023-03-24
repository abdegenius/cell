<script>
	let delete_modal = false;
	let edit_modal = false;
</script>

<div class="relative mx-auto max-w-7xl px-4 pb-12 sm:px-6 lg:px-8">
	<div>
		<dl
			class="mt-4 flex flex-col lg:flex-row space-y-4 lg:space-y-0 items-stretch justify-start divide-x-0 divide-y lg:divide-x lg:divide-y-0 divide-gray-300 bg-white border border-gray-300 rounded-md shadow-md drop-shadow-md"
		>
			<div class="w-full min-h-full lg:w-1/4 rounded-lg">
				<div class="p-4 bg-gray-100">
					<h3 class="mb-6 font-medium text-xl text-gray-600">Add new member</h3>
					<form class="space-y-4 overflow-y-auto scrollbar-hide" action="#" method="POST">
						<div>
							<div class="">
								<input
									type="text"
									required
									placeholder="First Name"
									class="block w-full rounded-md border-0 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-zinc-600 sm:text-sm sm:leading-6 p-2"
								/>
							</div>
						</div>
						<div>
							<div class="">
								<input
									type="text"
									required
									placeholder="Last Name"
									class="block w-full rounded-md border-0 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-zinc-600 sm:text-sm sm:leading-6 p-2"
								/>
							</div>
						</div>
						<div>
							<div class="">
								<input
									type="email"
									required
									placeholder="Email address"
									class="block w-full rounded-md border-0 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-zinc-600 sm:text-sm sm:leading-6 p-2"
								/>
							</div>
						</div>
						<div>
							<div class="">
								<input
									type="number"
									required
									placeholder="Phone Number"
									class="block w-full rounded-md border-0 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-zinc-600 sm:text-sm sm:leading-6 p-2"
								/>
							</div>
						</div>
						<div>
							<div class="">
								<p class="mb-0 text-[12px] font-normal text-gray-800">Date Of Birth</p>
								<input
									type="date"
									required
									class="block w-full rounded-md border-0 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-zinc-600 sm:text-sm sm:leading-6 p-2"
								/>
							</div>
						</div>
						<div>
							<div class="">
								<p class="mb-0 text-[12px] font-normal text-gray-800">Gender</p>
								<select
									required
									class="block w-full rounded-md border-0 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-zinc-600 sm:text-sm sm:leading-6 p-2"
								>
									<option value="male">Male</option>
									<option value="female">Female</option>
								</select>
							</div>
						</div>
						<div>
							<div class="">
								<input
									type="text"
									required
									placeholder="Address"
									class="block w-full rounded-md border-0 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-zinc-600 sm:text-sm sm:leading-6 p-2"
								/>
							</div>
						</div>

						<div>
							<button
								type="submit"
								class="flex w-full justify-center rounded-md bg-zinc-800 p-2 text-sm font-semibold text-white shadow-sm hover:bg-zinc-600 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-zinc-600"
								>Create New +</button
							>
						</div>
					</form>
				</div>
			</div>
			<div class="w-full lg:w-3/4 p-2 bg-gray-50">
				<div class="relative overflow-x-auto scrollbar-hide max-h-[600px]">
					<table class="relative w-full text-sm text-left text-gray-500">
						<thead class=" w-full text-xs text-gray-700 uppercase bg-gray-50">
							<tr>
								<th scope="col" class="p-2"> Personal Details </th>
								<th scope="col" class="p-2"> Contact Details</th>
								<th scope="col" class="p-2"> Action </th>
							</tr>
						</thead>
						<tbody class="pt-24 overflow-y-auto scrollbar-hide">
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										John Doe &nbsp;
										<span class="m-0 bg-gray-200 px-2 py-1 rounded-full w-fit font-bold">Male</span>
									</div>
									<div class="m-0 underline text-green-700">04-09-1999</div>
								</th>
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										+2340900024020 &nbsp; [<i class="m-0">john@doe.com</i>]
									</div>
									<div class="m-0">No. 5 Bama close, Barnawa, Kaduna South</div>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (edit_modal = true)}
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 focus:ring-4 focus:outline-none focus:ring-emerald-300 font-medium rounded-lg text-sm py-2 px-4 text-center "
										type="button"
									>
										<i class="fa fa-pencil fa-1x" />
									</button>
									<button
										on:click={() => (delete_modal = true)}
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 focus:ring-4 focus:outline-none focus:ring-rose-300 font-medium rounded-lg text-sm px-4 py-2 text-center"
										type="button"
									>
										<i class="fa fa-trash fa-1x" />
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										John Doe &nbsp;
										<span class="m-0 bg-gray-200 px-2 py-1 rounded-full w-fit font-bold">Male</span>
									</div>
									<div class="m-0 underline text-green-700">04-09-1999</div>
								</th>
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										+2340900024020 &nbsp; [<i class="m-0">john@doe.com</i>]
									</div>
									<div class="m-0">No. 5 Bama close, Barnawa, Kaduna South</div>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (edit_modal = true)}
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 focus:ring-4 focus:outline-none focus:ring-emerald-300 font-medium rounded-lg text-sm py-2 px-4 text-center "
										type="button"
									>
										<i class="fa fa-pencil fa-1x" />
									</button>
									<button
										on:click={() => (delete_modal = true)}
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 focus:ring-4 focus:outline-none focus:ring-rose-300 font-medium rounded-lg text-sm px-4 py-2 text-center"
										type="button"
									>
										<i class="fa fa-trash fa-1x" />
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										John Doe &nbsp;
										<span class="m-0 bg-gray-200 px-2 py-1 rounded-full w-fit font-bold">Male</span>
									</div>
									<div class="m-0 underline text-green-700">04-09-1999</div>
								</th>
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										+2340900024020 &nbsp; [<i class="m-0">john@doe.com</i>]
									</div>
									<div class="m-0">No. 5 Bama close, Barnawa, Kaduna South</div>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (edit_modal = true)}
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 focus:ring-4 focus:outline-none focus:ring-emerald-300 font-medium rounded-lg text-sm py-2 px-4 text-center "
										type="button"
									>
										<i class="fa fa-pencil fa-1x" />
									</button>
									<button
										on:click={() => (delete_modal = true)}
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 focus:ring-4 focus:outline-none focus:ring-rose-300 font-medium rounded-lg text-sm px-4 py-2 text-center"
										type="button"
									>
										<i class="fa fa-trash fa-1x" />
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										John Doe &nbsp;
										<span class="m-0 bg-gray-200 px-2 py-1 rounded-full w-fit font-bold">Male</span>
									</div>
									<div class="m-0 underline text-green-700">04-09-1999</div>
								</th>
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										+2340900024020 &nbsp; [<i class="m-0">john@doe.com</i>]
									</div>
									<div class="m-0">No. 5 Bama close, Barnawa, Kaduna South</div>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (edit_modal = true)}
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 focus:ring-4 focus:outline-none focus:ring-emerald-300 font-medium rounded-lg text-sm py-2 px-4 text-center "
										type="button"
									>
										<i class="fa fa-pencil fa-1x" />
									</button>
									<button
										on:click={() => (delete_modal = true)}
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 focus:ring-4 focus:outline-none focus:ring-rose-300 font-medium rounded-lg text-sm px-4 py-2 text-center"
										type="button"
									>
										<i class="fa fa-trash fa-1x" />
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										John Doe &nbsp;
										<span class="m-0 bg-gray-200 px-2 py-1 rounded-full w-fit font-bold">Male</span>
									</div>
									<div class="m-0 underline text-green-700">04-09-1999</div>
								</th>
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										+2340900024020 &nbsp; [<i class="m-0">john@doe.com</i>]
									</div>
									<div class="m-0">No. 5 Bama close, Barnawa, Kaduna South</div>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (edit_modal = true)}
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 focus:ring-4 focus:outline-none focus:ring-emerald-300 font-medium rounded-lg text-sm py-2 px-4 text-center "
										type="button"
									>
										<i class="fa fa-pencil fa-1x" />
									</button>
									<button
										on:click={() => (delete_modal = true)}
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 focus:ring-4 focus:outline-none focus:ring-rose-300 font-medium rounded-lg text-sm px-4 py-2 text-center"
										type="button"
									>
										<i class="fa fa-trash fa-1x" />
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										John Doe &nbsp;
										<span class="m-0 bg-gray-200 px-2 py-1 rounded-full w-fit font-bold">Male</span>
									</div>
									<div class="m-0 underline text-green-700">04-09-1999</div>
								</th>
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										+2340900024020 &nbsp; [<i class="m-0">john@doe.com</i>]
									</div>
									<div class="m-0">No. 5 Bama close, Barnawa, Kaduna South</div>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (edit_modal = true)}
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 focus:ring-4 focus:outline-none focus:ring-emerald-300 font-medium rounded-lg text-sm py-2 px-4 text-center "
										type="button"
									>
										<i class="fa fa-pencil fa-1x" />
									</button>
									<button
										on:click={() => (delete_modal = true)}
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 focus:ring-4 focus:outline-none focus:ring-rose-300 font-medium rounded-lg text-sm px-4 py-2 text-center"
										type="button"
									>
										<i class="fa fa-trash fa-1x" />
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										John Doe &nbsp;
										<span class="m-0 bg-gray-200 px-2 py-1 rounded-full w-fit font-bold">Male</span>
									</div>
									<div class="m-0 underline text-green-700">04-09-1999</div>
								</th>
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										+2340900024020 &nbsp; [<i class="m-0">john@doe.com</i>]
									</div>
									<div class="m-0">No. 5 Bama close, Barnawa, Kaduna South</div>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (edit_modal = true)}
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 focus:ring-4 focus:outline-none focus:ring-emerald-300 font-medium rounded-lg text-sm py-2 px-4 text-center "
										type="button"
									>
										<i class="fa fa-pencil fa-1x" />
									</button>
									<button
										on:click={() => (delete_modal = true)}
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 focus:ring-4 focus:outline-none focus:ring-rose-300 font-medium rounded-lg text-sm px-4 py-2 text-center"
										type="button"
									>
										<i class="fa fa-trash fa-1x" />
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										John Doe &nbsp;
										<span class="m-0 bg-gray-200 px-2 py-1 rounded-full w-fit font-bold">Male</span>
									</div>
									<div class="m-0 underline text-green-700">04-09-1999</div>
								</th>
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										+2340900024020 &nbsp; [<i class="m-0">john@doe.com</i>]
									</div>
									<div class="m-0">No. 5 Bama close, Barnawa, Kaduna South</div>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (edit_modal = true)}
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 focus:ring-4 focus:outline-none focus:ring-emerald-300 font-medium rounded-lg text-sm py-2 px-4 text-center "
										type="button"
									>
										<i class="fa fa-pencil fa-1x" />
									</button>
									<button
										on:click={() => (delete_modal = true)}
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 focus:ring-4 focus:outline-none focus:ring-rose-300 font-medium rounded-lg text-sm px-4 py-2 text-center"
										type="button"
									>
										<i class="fa fa-trash fa-1x" />
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										John Doe &nbsp;
										<span class="m-0 bg-gray-200 px-2 py-1 rounded-full w-fit font-bold">Male</span>
									</div>
									<div class="m-0 underline text-green-700">04-09-1999</div>
								</th>
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										+2340900024020 &nbsp; [<i class="m-0">john@doe.com</i>]
									</div>
									<div class="m-0">No. 5 Bama close, Barnawa, Kaduna South</div>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (edit_modal = true)}
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 focus:ring-4 focus:outline-none focus:ring-emerald-300 font-medium rounded-lg text-sm py-2 px-4 text-center "
										type="button"
									>
										<i class="fa fa-pencil fa-1x" />
									</button>
									<button
										on:click={() => (delete_modal = true)}
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 focus:ring-4 focus:outline-none focus:ring-rose-300 font-medium rounded-lg text-sm px-4 py-2 text-center"
										type="button"
									>
										<i class="fa fa-trash fa-1x" />
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										John Doe &nbsp;
										<span class="m-0 bg-gray-200 px-2 py-1 rounded-full w-fit font-bold">Male</span>
									</div>
									<div class="m-0 underline text-green-700">04-09-1999</div>
								</th>
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										+2340900024020 &nbsp; [<i class="m-0">john@doe.com</i>]
									</div>
									<div class="m-0">No. 5 Bama close, Barnawa, Kaduna South</div>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (edit_modal = true)}
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 focus:ring-4 focus:outline-none focus:ring-emerald-300 font-medium rounded-lg text-sm py-2 px-4 text-center "
										type="button"
									>
										<i class="fa fa-pencil fa-1x" />
									</button>
									<button
										on:click={() => (delete_modal = true)}
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 focus:ring-4 focus:outline-none focus:ring-rose-300 font-medium rounded-lg text-sm px-4 py-2 text-center"
										type="button"
									>
										<i class="fa fa-trash fa-1x" />
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										John Doe &nbsp;
										<span class="m-0 bg-gray-200 px-2 py-1 rounded-full w-fit font-bold">Male</span>
									</div>
									<div class="m-0 underline text-green-700">04-09-1999</div>
								</th>
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										+2340900024020 &nbsp; [<i class="m-0">john@doe.com</i>]
									</div>
									<div class="m-0">No. 5 Bama close, Barnawa, Kaduna South</div>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (edit_modal = true)}
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 focus:ring-4 focus:outline-none focus:ring-emerald-300 font-medium rounded-lg text-sm py-2 px-4 text-center "
										type="button"
									>
										<i class="fa fa-pencil fa-1x" />
									</button>
									<button
										on:click={() => (delete_modal = true)}
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 focus:ring-4 focus:outline-none focus:ring-rose-300 font-medium rounded-lg text-sm px-4 py-2 text-center"
										type="button"
									>
										<i class="fa fa-trash fa-1x" />
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										John Doe &nbsp;
										<span class="m-0 bg-gray-200 px-2 py-1 rounded-full w-fit font-bold">Male</span>
									</div>
									<div class="m-0 underline text-green-700">04-09-1999</div>
								</th>
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										+2340900024020 &nbsp; [<i class="m-0">john@doe.com</i>]
									</div>
									<div class="m-0">No. 5 Bama close, Barnawa, Kaduna South</div>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (edit_modal = true)}
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 focus:ring-4 focus:outline-none focus:ring-emerald-300 font-medium rounded-lg text-sm py-2 px-4 text-center "
										type="button"
									>
										<i class="fa fa-pencil fa-1x" />
									</button>
									<button
										on:click={() => (delete_modal = true)}
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 focus:ring-4 focus:outline-none focus:ring-rose-300 font-medium rounded-lg text-sm px-4 py-2 text-center"
										type="button"
									>
										<i class="fa fa-trash fa-1x" />
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										John Doe &nbsp;
										<span class="m-0 bg-gray-200 px-2 py-1 rounded-full w-fit font-bold">Male</span>
									</div>
									<div class="m-0 underline text-green-700">04-09-1999</div>
								</th>
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										+2340900024020 &nbsp; [<i class="m-0">john@doe.com</i>]
									</div>
									<div class="m-0">No. 5 Bama close, Barnawa, Kaduna South</div>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (edit_modal = true)}
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 focus:ring-4 focus:outline-none focus:ring-emerald-300 font-medium rounded-lg text-sm py-2 px-4 text-center "
										type="button"
									>
										<i class="fa fa-pencil fa-1x" />
									</button>
									<button
										on:click={() => (delete_modal = true)}
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 focus:ring-4 focus:outline-none focus:ring-rose-300 font-medium rounded-lg text-sm px-4 py-2 text-center"
										type="button"
									>
										<i class="fa fa-trash fa-1x" />
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										John Doe &nbsp;
										<span class="m-0 bg-gray-200 px-2 py-1 rounded-full w-fit font-bold">Male</span>
									</div>
									<div class="m-0 underline text-green-700">04-09-1999</div>
								</th>
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										+2340900024020 &nbsp; [<i class="m-0">john@doe.com</i>]
									</div>
									<div class="m-0">No. 5 Bama close, Barnawa, Kaduna South</div>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (edit_modal = true)}
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 focus:ring-4 focus:outline-none focus:ring-emerald-300 font-medium rounded-lg text-sm py-2 px-4 text-center "
										type="button"
									>
										<i class="fa fa-pencil fa-1x" />
									</button>
									<button
										on:click={() => (delete_modal = true)}
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 focus:ring-4 focus:outline-none focus:ring-rose-300 font-medium rounded-lg text-sm px-4 py-2 text-center"
										type="button"
									>
										<i class="fa fa-trash fa-1x" />
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										John Doe &nbsp;
										<span class="m-0 bg-gray-200 px-2 py-1 rounded-full w-fit font-bold">Male</span>
									</div>
									<div class="m-0 underline text-green-700">04-09-1999</div>
								</th>
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										+2340900024020 &nbsp; [<i class="m-0">john@doe.com</i>]
									</div>
									<div class="m-0">No. 5 Bama close, Barnawa, Kaduna South</div>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (edit_modal = true)}
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 focus:ring-4 focus:outline-none focus:ring-emerald-300 font-medium rounded-lg text-sm py-2 px-4 text-center "
										type="button"
									>
										<i class="fa fa-pencil fa-1x" />
									</button>
									<button
										on:click={() => (delete_modal = true)}
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 focus:ring-4 focus:outline-none focus:ring-rose-300 font-medium rounded-lg text-sm px-4 py-2 text-center"
										type="button"
									>
										<i class="fa fa-trash fa-1x" />
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										John Doe &nbsp;
										<span class="m-0 bg-gray-200 px-2 py-1 rounded-full w-fit font-bold">Male</span>
									</div>
									<div class="m-0 underline text-green-700">04-09-1999</div>
								</th>
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										+2340900024020 &nbsp; [<i class="m-0">john@doe.com</i>]
									</div>
									<div class="m-0">No. 5 Bama close, Barnawa, Kaduna South</div>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (edit_modal = true)}
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 focus:ring-4 focus:outline-none focus:ring-emerald-300 font-medium rounded-lg text-sm py-2 px-4 text-center "
										type="button"
									>
										<i class="fa fa-pencil fa-1x" />
									</button>
									<button
										on:click={() => (delete_modal = true)}
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 focus:ring-4 focus:outline-none focus:ring-rose-300 font-medium rounded-lg text-sm px-4 py-2 text-center"
										type="button"
									>
										<i class="fa fa-trash fa-1x" />
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										John Doe &nbsp;
										<span class="m-0 bg-gray-200 px-2 py-1 rounded-full w-fit font-bold">Male</span>
									</div>
									<div class="m-0 underline text-green-700">04-09-1999</div>
								</th>
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										+2340900024020 &nbsp; [<i class="m-0">john@doe.com</i>]
									</div>
									<div class="m-0">No. 5 Bama close, Barnawa, Kaduna South</div>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (edit_modal = true)}
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 focus:ring-4 focus:outline-none focus:ring-emerald-300 font-medium rounded-lg text-sm py-2 px-4 text-center "
										type="button"
									>
										<i class="fa fa-pencil fa-1x" />
									</button>
									<button
										on:click={() => (delete_modal = true)}
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 focus:ring-4 focus:outline-none focus:ring-rose-300 font-medium rounded-lg text-sm px-4 py-2 text-center"
										type="button"
									>
										<i class="fa fa-trash fa-1x" />
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										John Doe &nbsp;
										<span class="m-0 bg-gray-200 px-2 py-1 rounded-full w-fit font-bold">Male</span>
									</div>
									<div class="m-0 underline text-green-700">04-09-1999</div>
								</th>
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										+2340900024020 &nbsp; [<i class="m-0">john@doe.com</i>]
									</div>
									<div class="m-0">No. 5 Bama close, Barnawa, Kaduna South</div>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (edit_modal = true)}
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 focus:ring-4 focus:outline-none focus:ring-emerald-300 font-medium rounded-lg text-sm py-2 px-4 text-center "
										type="button"
									>
										<i class="fa fa-pencil fa-1x" />
									</button>
									<button
										on:click={() => (delete_modal = true)}
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 focus:ring-4 focus:outline-none focus:ring-rose-300 font-medium rounded-lg text-sm px-4 py-2 text-center"
										type="button"
									>
										<i class="fa fa-trash fa-1x" />
									</button>
								</th>
							</tr>
							<tr class="bg-white border border-gray-200">
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										John Doe &nbsp;
										<span class="m-0 bg-gray-200 px-2 py-1 rounded-full w-fit font-bold">Male</span>
									</div>
									<div class="m-0 underline text-green-700">04-09-1999</div>
								</th>
								<th scope="row" class="p-2 font-normal text-gray-900 whitespace-nowrap text-xs">
									<div class="m-0 text-md">
										+2340900024020 &nbsp; [<i class="m-0">john@doe.com</i>]
									</div>
									<div class="m-0">No. 5 Bama close, Barnawa, Kaduna South</div>
								</th>
								<th scope="col" class="p-2">
									<button
										on:click={() => (edit_modal = true)}
										class="m-1 inline-flex text-white bg-emerald-700 hover:bg-emerald-800 focus:ring-4 focus:outline-none focus:ring-emerald-300 font-medium rounded-lg text-sm py-2 px-4 text-center "
										type="button"
									>
										<i class="fa fa-pencil fa-1x" />
									</button>
									<button
										on:click={() => (delete_modal = true)}
										class="m-1 inline-flex text-white bg-rose-700 hover:bg-rose-800 focus:ring-4 focus:outline-none focus:ring-rose-300 font-medium rounded-lg text-sm px-4 py-2 text-center"
										type="button"
									>
										<i class="fa fa-trash fa-1x" />
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
	class="relative z-10 {delete_modal ? 'block' : 'hidden'}"
	aria-labelledby="modal-title"
	role="dialog"
	aria-modal="true"
>
	<div class="fixed inset-0 bg-gray-500 bg-opacity-75 transition-opacity" />

	<div class="fixed inset-0 z-10 overflow-y-auto">
		<div class="flex min-h-full items-end justify-center p-4 text-center sm:items-center sm:p-0">
			<div
				class="relative transform overflow-hidden rounded-lg bg-white px-4 pt-5 pb-4 text-left shadow-xl transition-all sm:my-8 sm:w-full sm:max-w-lg sm:p-6"
			>
				<div class="sm:flex sm:items-start">
					<div
						class="mx-auto flex h-12 w-12 flex-shrink-0 items-center justify-center rounded-full bg-red-100 sm:mx-0 sm:h-10 sm:w-10"
					>
						<svg
							class="h-6 w-6 text-red-600"
							fill="none"
							viewBox="0 0 24 24"
							stroke-width="1.5"
							stroke="currentColor"
							aria-hidden="true"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								d="M12 9v3.75m-9.303 3.376c-.866 1.5.217 3.374 1.948 3.374h14.71c1.73 0 2.813-1.874 1.948-3.374L13.949 3.378c-.866-1.5-3.032-1.5-3.898 0L2.697 16.126zM12 15.75h.007v.008H12v-.008z"
							/>
						</svg>
					</div>
					<div class="mt-3 text-center sm:mt-0 sm:ml-4 sm:text-left">
						<h3 class="text-base font-semibold leading-6 text-gray-900" id="modal-title">
							Delete Member
						</h3>
						<div class="mt-2">
							<p class="text-sm text-gray-500">
								Are you sure you want to delete this member? This action cannot be undone.
							</p>
						</div>
					</div>
				</div>
				<div class="mt-5 sm:mt-4 sm:ml-10 sm:flex sm:pl-4">
					<button
						type="button"
						class="inline-flex w-full justify-center rounded-md bg-red-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-red-500 sm:w-auto"
						>Delete</button
					>
					<button
						on:click={() => (delete_modal = false)}
						type="button"
						class="mt-3 inline-flex w-full justify-center rounded-md bg-white px-3 py-2 text-sm font-semibold text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 hover:bg-gray-50 sm:ml-3 sm:mt-0 sm:w-auto"
						>Cancel</button
					>
				</div>
			</div>
		</div>
	</div>
</div>

<div
	class="relative z-10 {edit_modal ? 'block' : 'hidden'}"
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
				<div class="mt-5">
					<div class="space-y-4 overflow-y-auto scrollbar-hide">
						<div>
							<div class="">
								<input
									type="text"
									required
									placeholder="First Name"
									class="block w-full rounded-md border-0 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-zinc-600 sm:text-sm sm:leading-6 p-2"
								/>
							</div>
						</div>
						<div>
							<div class="">
								<input
									type="text"
									required
									placeholder="Last Name"
									class="block w-full rounded-md border-0 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-zinc-600 sm:text-sm sm:leading-6 p-2"
								/>
							</div>
						</div>
						<div>
							<div class="">
								<input
									type="email"
									required
									placeholder="Email address"
									class="block w-full rounded-md border-0 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-zinc-600 sm:text-sm sm:leading-6 p-2"
								/>
							</div>
						</div>
						<div>
							<div class="">
								<input
									type="number"
									required
									placeholder="Phone Number"
									class="block w-full rounded-md border-0 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-zinc-600 sm:text-sm sm:leading-6 p-2"
								/>
							</div>
						</div>
						<div>
							<div class="">
								<p class="mb-0 text-[12px] font-normal text-gray-800">Date Of Birth</p>
								<input
									type="date"
									required
									class="block w-full rounded-md border-0 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-zinc-600 sm:text-sm sm:leading-6 p-2"
								/>
							</div>
						</div>
						<div>
							<div class="">
								<p class="mb-0 text-[12px] font-normal text-gray-800">Gender</p>
								<select
									required
									class="block w-full rounded-md border-0 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-zinc-600 sm:text-sm sm:leading-6 p-2"
								>
									<option value="male">Male</option>
									<option value="female">Female</option>
								</select>
							</div>
						</div>
						<div>
							<div class="">
								<input
									type="text"
									required
									placeholder="Address"
									class="block w-full rounded-md border-0 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-zinc-600 sm:text-sm sm:leading-6 p-2"
								/>
							</div>
						</div>
					</div>
				</div>

				<div class="mt-5">
					<button
						type="button"
						class="inline-flex w-full justify-center rounded-md bg-emerald-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-emerald-500 sm:w-auto"
						>Save Changes</button
					>
					<button
						on:click={() => (edit_modal = false)}
						type="button"
						class="mt-3 inline-flex w-full justify-center rounded-md bg-white px-3 py-2 text-sm font-semibold text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 hover:bg-gray-50 sm:ml-3 sm:mt-0 sm:w-auto"
						>Cancel</button
					>
				</div>
			</div>
		</div>
	</div>
</div>
