<script>
	import Carousel from './Carousel.svelte';
	import Skill from './Skill.svelte';
</script>



<main  >

	<!-- INIT -->
	<div class="me">
		<div class="me-bg"></div>
		<span class="text" id="title">
			Soy creador de sitios web y aplicaciones
		</span>
	</div>

	<div>
		<svg version="1.1" class="arrow-down" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
			viewBox="0 0 21.825 21.825">
		<path d="M16.791,13.254c0.444-0.444,1.143-0.444,1.587,0c0.429,0.444,0.429,1.143,0,1.587l-6.65,6.651
			c-0.206,0.206-0.492,0.333-0.809,0.333c-0.317,0-0.603-0.127-0.81-0.333l-6.65-6.651c-0.444-0.444-0.444-1.143,0-1.587
			s1.143-0.444,1.587,0l4.746,4.762V1.111C9.791,0.492,10.299,0,10.918,0c0.619,0,1.111,0.492,1.111,1.111v16.904L16.791,13.254z"/>
		</svg>
	</div>


	<!-- SOBRE MI -->
	<div class="data">
		<svg class="icon" viewBox="0 0 512 512" xmlns="http://www.w3.org/2000/svg"><g><g><path d="m433 512c-11.046 0-20-8.954-20-20 0-78.299-63.701-142-142-142h-30c-78.299 0-142 63.701-142 142 0 11.046-8.954 20-20 20s-20-8.954-20-20c0-100.355 81.645-182 182-182h30c100.355 0 182 81.645 182 182 0 11.046-8.954 20-20 20z"/></g><g><path d="m254 270c-74.439 0-135-60.561-135-135s60.561-135 135-135 135 60.561 135 135-60.561 135-135 135zm0-230c-52.383 0-95 42.617-95 95s42.617 95 95 95 95-42.617 95-95-42.617-95-95-95z"/></g></g></svg>
		<h2 class="title">Sobre mi</h2>
		<span class="text">
			Mi nombre es David y soy  un apasionado por la tecnologia,
			me encanta crear experiencias increibles y me especializo en la
			creacion y el diseño de <h1><strong>Aplicaciones Moviles</strong></h1>,
			<strong>Web</strong> y de <strong>Escritorio</strong>
			puedo convertir tu idea de un negocio en realidad.
			si quieres ver un poco de mi
			trabajo puedes mirarlo más abajo.
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
			¿Quieres crear una aplicaciones o un sitio web? o tan solo te gustaria
			conocer el costo aproximado, mandame un correo
			<a class="url" href="mailto:david_xd1996@live.com.mx">Aqui</a>.
			¿Te gustaria saber que habilidades tengo? puedes ver mi CV
			<a class="url" href="mailto:david_xd1996@live.com.mx">Aqui</a>. 
		</span>
	</div>



	<!-- PORTAFOLIO -->
	<div class="data" >
		<h2 class="title">Portafolio</h2>
		<div class="proyect">
			<Carousel />
		</div>
	</div>

	

	<!-- MIS HABILIDADES -->
	<div class="data">
		<h2 class="title">Habilidades</h2>
		<span class="text content">
			<Skill data={[8, 'fab fa-python',    'python']} />
			<Skill data={[7, 'csharp',           'c#']} />
			<Skill data={[9, 'fab fa-git-alt',    'git']} />
			<Skill data={[7, 'fab fa-github',    'github']} />
			<Skill data={[9, 'fab fa-html5',     'html5']} />
			<Skill data={[7, 'fab fa-js-square', 'js']} />
			<Skill data={[7, 'fab fa-css3-alt',  'css3']} />
			<Skill data={[7, 'fab fa-sass',      'sass']} />
			<Skill data={[6, 'fab fa-bootstrap', 'bootstrap']} />
			<Skill data={[7, 'svelte',           'svelte']} />
			<Skill data={[6, 'fab fa-react',     'react']} />
			<Skill data={[7, 'fab fa-node-js',   'node']} />
			<Skill data={[7, 'fas fa-database',  'SQL']} />
			<Skill data={[8, 'fab fa-npm',       'npm']} />
		</span>
		<h2 class="title">Estoy aprendiendo</h2>
		<span class="text content">
			<Skill data={[0, 'xd',  'xd']} />
			<Skill data={[0, 'xd ', 'xd']} />
		</span>
	</div>
	
	<!-- MIS SERVICIOS -->
	<div class="data">
		<h2 class="title">Servicios</h2>
		<span class="text">
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

	#title {
		z-index: 50;
		position: absolute;
		text-shadow:  2px 2px var(--background);
		font-size: 1.7rem;
		font-weight: 600;
		text-align: center;
	}

	h1 {
		display: inline;
		font-size: 1rem;
		font-family: sans-serif;
		font-weight: 100;
	}

	.arrow-down {
		margin: 3rem 0;
		fill: var(--color-icon);
		width: 50px;
		animation: gradient 3s infinite;
	}

	@keyframes gradient {
        0% {
            fill: #fff;
        }
        35% {
            fill:var(--color-icon);
        }
        65% {
            fill:var(--color-icon);
        }
		100% {
            fill: #fff;
		}
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
		filter: blur(4px);
		width: 100%;
		height: 100%;
		opacity: .3;
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
		margin: 2rem 0;
		width: 100%;
	}

	.icon {
		width: 45px;
		height: 45px;
		background-color: var(--background2);
		border-radius: 50%;
		padding: 15px;
		fill: var(--color-icon);
	}

	.url:link, .url:active, .url:visited {
		color: var(--color-icon);
		text-decoration: none;
	}

	.portafolio {
		display: flex;
		/* align-items: center; */
		/* justify-content: flex-start; */
		width: 100%;
		margin: 0 1.5rem;
		/* flex: 1; */
		flex-wrap: wrap;
	}

	.proyect {
		width: 100%;
	}


	.content {
		display: flex;
		flex-wrap: wrap;
		justify-content:space-between;
		align-items: flex-start;
	}













</style>