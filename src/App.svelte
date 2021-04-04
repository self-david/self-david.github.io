<script>
	import Loading from './components/Loading.svelte';
	import Header from './components/Header.svelte';
	import Main from './components/Main.svelte';
	import Redes from './components/Redes.svelte';
	import Footer from './components/Footer.svelte';
    const navbar = ['sobre mi', 'contacto', 'portafolio', 'habilidades', 'curriculum'];

</script>

<Loading />
<Header navBar={navbar}/>

<Main element={navbar}/>


<Redes />
<Footer />

<style>

</style>