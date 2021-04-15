<script>
	import Loading from './components/Loading.svelte';
	import Header from './components/Header.svelte';
	import Main from './components/Main.svelte';
	import Redes from './components/Redes.svelte';
	import Footer from './components/Footer.svelte';
    
	const cssVar = {
		background : "#14162C",
		background2 : "#39385D",
		white : "#FFFFFF",
		gray : "#EEEEFF",
		red : "#FF1133",
		violet : "#DA77FF",
	};


</script>

<Loading cssVar={cssVar} />
<Header cssVar={cssVar} />

<!-- <img class="dos" src="./assets/desing/logo.svg" alt=""> -->

<Main cssVar={cssVar} />


<Redes />
<Footer />

<style>
	:root {
		--background: #14162C;
		font-size: 16px;
	}

</style>