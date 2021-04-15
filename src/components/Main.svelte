<script>
	export let cssVar;
</script>



<main  style="--background: {cssVar.background};
			  --background2: {cssVar.background2};
	 		  --violet: {cssVar.violet};
	 		  --red: {cssVar.red};">

	
	<!-- SOBRE MI -->
	<div class="me" style="--background: {cssVar.background};">
		<div class="me-bg"></div>
		<span class="text me-text">
			Mi nombre es <h1>David</h1> y soy desarrollador
			de software, si estas interesado en alguna
			aplicación o si tan solo quieres ver un poco de mi
			trabajo puedes mirarlo más abajo.</span>

	</div>



	<!-- SOBRE MI -->
	<div class="data">
		<svg class="icon" viewBox="0 0 512 512" xmlns="http://www.w3.org/2000/svg"><g><g><path d="m433 512c-11.046 0-20-8.954-20-20 0-78.299-63.701-142-142-142h-30c-78.299 0-142 63.701-142 142 0 11.046-8.954 20-20 20s-20-8.954-20-20c0-100.355 81.645-182 182-182h30c100.355 0 182 81.645 182 182 0 11.046-8.954 20-20 20z"/></g><g><path d="m254 270c-74.439 0-135-60.561-135-135s60.561-135 135-135 135 60.561 135 135-60.561 135-135 135zm0-230c-52.383 0-95 42.617-95 95s42.617 95 95 95 95-42.617 95-95-42.617-95-95-95z"/></g></g></svg>
		<h2 class="title">Sobre mi</h2>
		<span class="text">
			soy un apasionado de la tecnologia y me encanta  crear vida en internet.
			Me especializo en crear (y ocacionalmente en diseñar)
			<strong>Aplicaciones Web</strong> y <strong>Aplicaciones De Escritorio</strong>
			puedo convertir tu idea de un negocio en realidad.
		</span>
	</div>


	<!-- CONTACTO -->
	<div class="data">
		<svg version="1.1" class="icon" xmlns="http://www.w3.org/2000/svg" viewBox="-70 -70 652 652" xmlns:xlink="http://www.w3.org/1999/xlink">
			<path d="M467,76H45C20.137,76,0,96.262,0,121v270c0,24.885,20.285,45,45,45h422c24.655,0,45-20.03,45-45V121
						C512,96.306,491.943,76,467,76z M460.698,106c-9.194,9.145-167.415,166.533-172.878,171.967c-8.5,8.5-19.8,13.18-31.82,13.18
						s-23.32-4.681-31.848-13.208C220.478,274.284,64.003,118.634,51.302,106H460.698z M30,384.894V127.125L159.638,256.08L30,384.894z
						 M51.321,406l129.587-128.763l22.059,21.943c14.166,14.166,33,21.967,53.033,21.967c20.033,0,38.867-7.801,53.005-21.939
						l22.087-21.971L460.679,406H51.321z M482,384.894L352.362,256.08L482,127.125V384.894z"/>
			</svg>
		<h2 class="title">Contacto</h2>
		<span class="text">
			soy un apasionado de la tecnologia y me encanta  crear vida en internet.
			Me especializo en crear (y ocacionalmente en diseñar)
			<strong>Aplicaciones Web</strong> y <strong>Aplicaciones De Escritorio</strong>
			puedo convertir tu idea de un negocio en realidad.
		</span>
	</div>



	<!-- PORTAFOLIO -->
	<div class="card" >
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
	<div class="card">
		<h2 class="title">habilidades</h2>
		<span class="justify">
			Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequuntur, quibusdam sunt, dignissimos reiciendis voluptate nihil iusto facere, laborum incidunt sint fuga accusantium eius sequi illum nemo quaerat aspernatur consectetur praesentium.
		</span>
	</div>
	


</main>


<style>
	main {
		background: var(--background);
		display: flex;
		align-items: center;
		justify-content: center;
		flex-direction: column;
	}

	h1 {
		display: inline;
		font-size: 1rem;
		font-family: sans-serif;
		font-weight: 100;
	}

	.me {
		width: 100vw;
		height: 375px;
		display: flex;
		align-items: center;
		justify-content: center;
		font-family: monospace;
	}

	.me-bg {
		background: url("../assets/imgbg.jpg")
					no-repeat
					center
					center/cover;
		filter: blur(5px);
		width: 100%;
		height: 100%;
		opacity: .25;
	}

	.me-text {
		z-index: 50;
		position: absolute;
		text-shadow:  2px 2px var(--background);
	}

	.text {
		font-size: 1em;
		font-family: sans-serif;
		font-weight: 100;
		margin: 0 1.5rem;
		text-align: justify;
	}

	.data {
		display: flex;
		align-items: center;
		justify-content: center;
		flex-direction: column;
		margin: 3rem 0;
	}

	.icon {
		width: 45px;
		height: 45px;
		background-color: var(--background2);
		border-radius: 50%;
		padding: 15px;
		fill: var(--violet);
	}





</style>