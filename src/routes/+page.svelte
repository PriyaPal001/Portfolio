<script>
	import Skills from '$lib/components/skills.svelte';
    import Prosec from '$lib/components/projects.svelte';
    import Dashboard from '$lib/components/dashboard.svelte';
    import Contact from '$lib/components/contact.svelte';
    import Footer from '$lib/components/footer.svelte';
    import Navbar from '$lib/components/nav.svelte';
    
	
</script>

<div class="bg-black h-screen">
    <Navbar/>
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


<style>
    @import url("https://fonts.googleapis.com/css2?family=Great+Vibes&display=swap");

:global(.logo) {
  font-family: "Great Vibes", cursive;
  font-size: 2rem;
}
</style>