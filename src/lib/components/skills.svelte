<script>
    import svelte from '$lib/images/skills/svelte.svg'
    import tw from '$lib/images/skills/tw.svg'
    import supa from '$lib/images/skills/supa.svg'
    import sass from '$lib/images/skills/sass.svg'
    import react from '$lib/images/skills/react.svg'
    import node from '$lib/images/skills/node.svg'
    import mongo from '$lib/images/skills/mongo.svg'
    import js from '$lib/images/skills/js.svg'
    import html from '$lib/images/skills/html.svg'
    import git from '$lib/images/skills/git.svg'
    import github from '$lib/images/skills/github.svg'
    import express from '$lib/images/skills/express.svg'
    import css from '$lib/images/skills/css.svg'
	let poppy = [
		{
			skills: 'SVELTE',
            icon: svelte
		},
        {
            skills: 'TAILWINDCSS',
            icon: tw
        },
        {
            skills:'SUPABASE',
            icon: supa
        },
        {
            skills: 'REACT',
            icon: react
        },
        {
            skills: 'JAVASCRIPT',
            icon: js
        },
        {
            skills: 'HTML',
            icon: html
        },
        {
            skills: 'CSS',
            icon: css
        },
        {
            skills: 'SASS',
            icon: sass
        },
        {
            skills: 'NODEJS',
            icon: node
        },
        {
            skills: 'EXPRESS',
            icon: express
        },
        {
            skills: 'MONGODB',
            icon: mongo
        },
        {
            skills: 'GIT',
            icon: git
        },
        {
            skills: 'GITHUB',
            icon: github
        },
        

	];
</script>

<section class="bg-black text-slate-300" id="skills">
	<div class=" w-full px-2 py-8 sm:px-4 sm:py-8 lg:px-32 lg:py-8">
		<span class="flex items-center">
            <span class="pr-2 text-5xl font-bold">Skills</span>
            <span class="h-px mt-4 flex-1 bg-slate-500"></span>
          </span>

          <!-- <div class="mx-auto max-w-lg text-center">
            <h2 class="text-3xl font-bold sm:text-4xl">Skills</h2>
          </div> -->

		<div class="mt-20 flex flex-wrap place-items-center gap-x-10 gap-y-10">
			{#each poppy as i}
            <a href="#" class="flex ">
                    <img src={i.icon} alt="" class="mx-2 h-8 w-8 flex items-center justify-center">
					<h2 class="mt-0 text-xl font-normal hover:text-white hover:underline hover:underline-offset-8 text-white">{i.skills}</h2>
				</a>
			{/each}
		</div>
	</div>
</section>

<!-- grid grid-cols-1 gap-6 md:grid-cols-2 lg:grid-cols-5 -->
