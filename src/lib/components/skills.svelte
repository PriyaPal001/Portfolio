<script>
	let poppy = [
		{
			skills: 'SVELTE'
		},
        {
            skills: 'TAILWINDCSS'
        },
        {
            skills:'SUPABASE'
        },
        {
            skills: 'REACT'
        },
        {
            skills: 'JAVASCRIPT'
        },
        {
            skills: 'HTML'
        },
        {
            skills: 'CSS'
        },
        {
            skills: 'NODEJS'
        },
        {
            skills: 'EXPRESS'
        },
        {
            skills: 'MONGODB'
        },
        {
            skills: 'GIT'
        },
        {
            skills: 'GITHUB'
        },
        

	];
</script>

<section class="bg-black text-white" id="skills">
	<div class="mx-auto max-w-screen-lg px-2 py-8 sm:px-4 sm:py-8 lg:px-4 lg:py-8">
		<!-- <span class="flex items-center">
            <span class="pr-2 text-3xl font-bold">Lorem, ipsum dolor</span>
            <span class="h-px flex-1 bg-white"></span>
          </span> -->

          <div class="mx-auto max-w-lg text-center">
            <h2 class="text-3xl font-bold sm:text-4xl">Skills</h2>
          </div>

		<div class="mt-8 grid grid-cols-1 gap-6 md:grid-cols-2 lg:grid-cols-5">
			{#each poppy as i}
				<a href="#">
					<h2 class="mt-0 text-xl font-normal hover:text-white hover:underline hover:underline-offset-8 text-white">{i.skills}</h2>
				</a>
			{/each}
		</div>
	</div>
</section>
