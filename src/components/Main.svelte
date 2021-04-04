<script>
	export let element;
</script>


<main>
	<!-- SOBRE MI -->
	<div class="me">
		<img class="photo" src="./assets/pp.jfif" alt="david gutierrez alvarez">
		<span class="center">
			<p class="me-text">Mi nombre es</p>
			<h1 class="me__name">david gutierrez alvarez</h1>
			<p class="me-text">- Desarrollador De Software -</p>
		</span>
	</div>


	<!-- SOBRE MI -->
	<div class="card" id={element[0]}>
		<h2 class="title">sobre mi</h2>
		<span class="justify">
			soy un apasionado de la tecnologia y me encanta  crear vida en internet.
			Me especializo en crear (y ocacionalmente en diseñar)
			<strong>Aplicaciones Web</strong> y <strong>Aplicaciones De Escritorio</strong>
			puedo convertir tu idea de un negocio en realidad.
		</span>
	</div>


	<!-- CONTACTO -->
	<div class="card" id={element[1]}>
		<h2 class="title">contacto</h2>
		<span class="justify">
			te gustaria cotizar algun proyecto sin compromiso, puedes mandarme un correo haciendo
			click
			<a class="link" href="mailto:david_xd1996@live.com.mx">aqui</a>.
		</span>
	</div>


	<!-- PORTAFOLIO -->
	<div class="card" id={element[2]}>
		<h2 class="title">portafolio</h2>
		<div class="portafolio">
			<div>proyecto 1</div>
			<div>proyecto 2</div>
			<div>proyecto 3</div>
			<div>proyecto 4</div>
			<div>proyecto 5</div>
			<div>proyecto 6</div>
			<div>proyecto 7</div>
			<div>proyecto 8</div>
			<div>proyecto 9</div>
			<div>proyecto...</div>
		</div>
	</div>
	

		<!-- MIS HABILIDADES -->
		<div class="card" id={element[3]}>
			<h2 class="title">habilidades</h2>
			<span class="justify">
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequuntur, quibusdam sunt, dignissimos reiciendis voluptate nihil iusto facere, laborum incidunt sint fuga accusantium eius sequi illum nemo quaerat aspernatur consectetur praesentium.
			</span>
		</div>
	


<!-- CURRICULUM -->

</main>


<style>
	main {
		/* background-color: teal; */
		display: flex;
		align-items: center;
		justify-content: center;
		flex-direction: column;
		margin: 1.5rem 2rem;
	}

	.me {
		display: flex;
		align-items: center;
		justify-content: center;
		flex-direction: column;
		text-align: center;
		margin: 2.3rem 0;
		font-family: monospace;
	}

	.photo {
		border-radius: 50%;
		height: 200px;
		filter: grayscale(1);
		margin-bottom: 1rem;
		z-index: -1;
	}

	.photo:hover {
		filter: grayscale(0);
	}

	.me-text {
		margin: 5px;
		font-size: 1rem;
	}

	.me__name {
		text-transform: uppercase;
		display: inline;
		font-size: 1.5rem;
		color: #f50;
	}

	.card {
		/* border: 1px solid #4981B8; */
		border-radius: 3px;
		/* background-color: rebeccapurple; */
		padding: 15px;
		margin: 0 0 10rem;
	}

	/* .title {
		display: flex;
		align-items: center;
		justify-content:space-between;
		flex-direction: column;
		text-transform: uppercase;
	}

	.title::after {
		content: "";
		display: inline-block;
		width: 100%;
		height: 1px;
		margin: 1rem 0 .5rem;
		background-color: #f50;
	} */

	.title {
		display: flex;
		align-items: center;
		justify-content:space-between;
		text-transform: uppercase;
	}

	.title::after {
		content: "";
		display: inline-block;
		width: 55%;
		height: 1px;
		margin: 1rem 0 .5rem;
		/* background-color: #4981B8; */
		background-color: #f50;
	}

	.portafolio {
		display: flex;
		align-items: center;
		justify-content:center;
		/* flex-direction: column; */
  flex-wrap: wrap;
	}


	.link, .link:link, .link:visited, .link:active {
		color: #4981B8;
		text-decoration: none;
	}



	.justify {
		font-size: 1rem;
		text-align: justify;
		display: block;
	}

	.justify::first-letter {
		text-transform: uppercase;
	}

	.center {
		text-align: center;
	}

</style>