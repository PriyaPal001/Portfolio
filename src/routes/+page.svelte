<script>
	import Skills from '$lib/components/skills.svelte';
    import Prosec from '$lib/components/projects.svelte';
    import Dashboard from '$lib/components/dashboard.svelte';
    import Contact from '$lib/components/contact.svelte';
    import Footer from '$lib/components/footer.svelte';
    import Navbar from '$lib/components/nav.svelte';
    
	
</script>

<div class="bg-black ">
   
    <main>
        <Dashboard />
        <Skills/>
        <Prosec/>
        <Contact/>
    </main>
    <footer>
        <Footer/>
    </footer>
</div>
