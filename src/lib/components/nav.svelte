<script>
	import { slide } from 'svelte/transition';
	import m1 from '$lib/images/home.svg';
	import m2 from '$lib/images/about.svg';
	import m3 from '$lib/images/skills.svg';
	import m4 from '$lib/images/project.svg';
	import m5 from '$lib/images/contact.svg';

	let navs = [
		{
			name: 'Home',
			link: '/',
			micon: m1
		},
		{
			name: 'About',
			link: '#about',
			micon: m2
		},
		{
			name: 'Skills',
			link: '#skills',
			micon: m3
		},
		{
			name: 'Projects',
			link: '#projects',
			micon: m4
		},
		{
			name: 'Contact',
			link: '#contact',
			micon: m5
		}
	];
	let mobile = false;
</script>

<nav class="sticky top-0 z-50 border-b border-slate-500 bg-black md:-mt-20">
	<div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
		<div class="relative flex h-16 items-center justify-between">
			<div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
				<!-- Mobile menu button-->
				<button
					type="button"
					class="relative inline-flex items-center justify-center rounded-md p-2 text-gray-400 hover:bg-black hover:text-white focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white"
					aria-controls="mobile-menu"
					aria-expanded="false"
					on:click={() => (mobile = !mobile)}
				>
					<span class="absolute -inset-0.5"></span>
					<span class="sr-only">Open main menu</span>
					<!--
                    Icon when menu is closed.
        
                    Menu open: "hidden", Menu closed: "block"
                  -->
					<svg
						class="{mobile ? 'hidden' : 'block'} h-6 w-6"
						fill="none"
						viewBox="0 0 24 24"
						stroke-width="1.5"
						stroke="currentColor"
						aria-hidden="true"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
						/>
					</svg>
					<!--
                    Icon when menu is open.
        
                    Menu open: "block", Menu closed: "hidden"
                  -->
					<svg
						class="{mobile ? 'block' : 'hidden'} h-6 w-6"
						fill="none"
						viewBox="0 0 24 24"
						stroke-width="1.5"
						stroke="currentColor"
						aria-hidden="true"
					>
						<path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
					</svg>
				</button>
			</div>
			<div class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-start">
				<!-- <div class="flex flex-shrink-0 items-center">
                        <lord-icon
                        src={iconn}
                        trigger="loop"
                        state="in-reveal"
                        delay="2000"
                        style="height:40px;width:40px;"
                    >
                      </div> -->
				<div class="m-0 flex h-8 w-12 p-0">
					<div class="mx-0 flex gap-x-2 border-white px-2">
						<!-- <img src={iconn} alt="" /> -->
						<span class="logo text-white">P</span>
						<span class="logo text-white">P</span>
						<!-- <img src={iconn} alt="" /> -->
					</div>
				</div>
				<div class="hidden w-full sm:ml-6 sm:block">
					<div class="flex justify-center space-x-4">
						{#each navs as item}
							<a
								href={item.link}
								class="rounded-md px-3 py-2 text-sm font-medium text-gray-300 hover:text-white hover:underline hover:underline-offset-8"
								>{item.name}</a
							>
						{/each}
					</div>
				</div>
				<div class="hidden items-center justify-center sm:flex">
					<ul class="flex items-center justify-center gap-x-4 text-white hover:cursor-pointer">
						<li>
							<a href="mailto:priyapal240302@gmail.com"
								><svg
									xmlns="http://www.w3.org/2000/svg"
									width="24"
									height="24"
									viewBox="0 0 24 24"
									fill="none"
									stroke="currentColor"
									stroke-width="2"
									stroke-linecap="round"
									stroke-linejoin="round"
									class="lucide lucide-mail"
									><rect width="20" height="16" x="2" y="4" rx="2" /><path
										d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"
									/></svg
								></a
							>
						</li>
						<li>
							<a href="https://github.com/PriyaPal001" target="_blank">
								<svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
									<path
										fill-rule="evenodd"
										d="M12 2C6.477 2 2 6.484 2 12.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.202 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0022 12.017C22 6.484 17.522 2 12 2z"
										clip-rule="evenodd"
									/>
								</svg></a
							>
						</li>
						<li>
							<a href="https://www.linkedin.com/in/priya-bidyut-pal/" target="_blank">
								<svg
									xmlns="http://www.w3.org/2000/svg"
									width="24"
									height="24"
									viewBox="0 0 24 24"
									fill="white"
									stroke="currentColor"
									stroke-width="2"
									stroke-linecap="round"
									stroke-linejoin="round"
									class="lucide lucide-linkedin"
									><path
										d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"
									/><rect width="4" height="12" x="2" y="9" /><circle cx="4" cy="4" r="2" /></svg
								>
							</a>
						</li>
					</ul>
				</div>
			</div>
		</div>
	</div>

	<!-- Mobile menu, show/hide based on menu state. -->
	{#key mobile}
		<div class="bg-black sm:hidden {mobile ? 'block' : 'hidden'}" id="mobile-menu" in:slide>
			<div class="space-y-1 px-2 pb-3 pt-2">
				{#each navs as item}
					<a
						href={item.link}
						class="flex items-center rounded-md px-3 py-2 text-base font-medium text-gray-300 hover:bg-black hover:text-white hover:underline hover:underline-offset-8"
						><img src={item.micon} alt={item.name} class="mr-5" />{item.name}</a
					>
				{/each}
			</div>
		</div>
	{/key}
</nav>
