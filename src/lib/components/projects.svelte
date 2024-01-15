<script>
    
  import AOS from "aos";
  import "aos/dist/aos.css"; // You can also use <link> for styles
  import { onMount } from "svelte";
  // ..
  onMount(() => {
    AOS.init();
  });
    let poppy=[
        {   
            icon:"D",
            title:"Dream Dress",
            description:"A e-commerce website for a fashion designer to showcase her designs and also to rent the products. The website is built with Svete and Tailwindcss.",
            link:"https://dream-dress.vercel.app"
        },
        {
            icon:"B",
            title:"BlogVlog",
            description:"This is a blog website built with svelte and tailwindcss. It is a blog website that allows users to create and read blogs.",
            link:"https://blog-vlog.vercel.app"
        },
        {
            icon:"T",
            title:"Todo List",
            description:"Svelte todo list app with local storage. This is a todo list app built with svelte and tailwindcss. It allows users to create, read, update and delete todos.",
            link:"https://priyapal001.github.io/Creative-Todo/"
        },
        {
            icon:"G",
            title:"Game",
            description:"It's a dragon game buit with react and tailwindcss. It's a game where you have to kill the dragon before it kills you.",
            link:"dragon-game-phi.vercel.app"
        },
        {
            icon:"I",
            title:"ImgToUrl",
            description:"This is a website that allows users to convert images to url. It is built with svelte and tailwindcss.",
            link:"imagify-beryl.vercel.app"
        },
        {
            title:"Digital campaigns",
            description:"Lorem ipsum dolor sit amet consectetur adipisicing elit. Ex ut quo possimus adipisci distinctio alias voluptatum blanditiis laudantium.",
        },
    ]
</script>

<section class="bg-black text-white " id="projects">
    <div class="mx-auto max-w-screen-xl px-4 py-8 sm:px-6 sm:py-12 lg:px-8 lg:py-16">
      <span class="flex items-center">
        <span class="pr-2 text-5xl font-bold">Projects</span>
        <span class="h-px mt-4 flex-1 bg-slate-500"></span>
      </span>
      <!-- <div class="mx-auto max-w-lg text-center">
        <h2 class="text-3xl font-bold sm:text-4xl">Projects</h2>
      </div> -->
  
      <div class="mt-20 grid grid-cols-1 gap-8  md:grid-cols-2 lg:grid-cols-3 " >
        {#each poppy as i,index}
        <a
        class="block rounded-xl border border-gray-800 p-8 shadow-xl transition hover:border-white/10 hover:shadow-white/10"
        href="{i.link}"
        data-aos="fade-up" data-aos-delay={(index+1)*150} data-aos-duration="800"
        >
        <!--Add in the class above hover:border-pink-500/10 hover:shadow-pink-500/10  -->
        <!-- <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-10 w-10 text-white"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path d="M12 14l9-5-9-5-9 5 9 5z" />
          <path
            d="M12 14l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14z"
          />
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M12 14l9-5-9-5-9 5 9 5zm0 0l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14zm-4 6v-7.5l4-2.222"
          />
        </svg> -->
        <span class="h-10 w-10 text-white logo">{i.icon}</span>

        <h2 class="mt-4 text-xl font-bold text-white">{i.title}</h2>

        <p class="mt-1 text-sm text-gray-300">
         {i.description}
        </p>
      </a>
        {/each}
  
      </div>

    </div>
  </section>