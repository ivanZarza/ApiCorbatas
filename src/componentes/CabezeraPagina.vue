<script setup>

</script>

<template>

	<div class="container">

		<img src="../../public/personal.jpg" class="personal">

		<div class="texto">
			<h1 class="text-center">De un Sueño a una Realidad. </h1>
			<p>
				Siempre soñé con pertenecer al mundo de la moda, con tener un nombre que la gente conociese, con crear una marca
				propia y dar a demostrar a la gente lo que puedo llegar a hacer con mi imaginación.
				<br>
				Hoy, todo ese sueño se ha convertido en una realidad, por primera vez puedo mostrar al mundo que gracias a mucho
				esfuerzo, constancia y perseverancia los sueños se hacen realidad y yo estoy cumpliendo el mío.
				Desde aquí ánimo a todas esas personas que tienen sueños que luchen por conseguirlos.
				<br>
				Os presento mi primera colección en la cual fusiono El Arte, La Cultura y El Flamenco. Tres características que
				me identifican por completo.
			</p>
		</div>
	</div>

</template>

<style scoped>
:root {
	height: 100%;
	width: 100%;
}

.container {
	width: 80;
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: center;
	gap: 5px;
	opacity: 0.7;
	margin: 20px;
}

.personal {
	min-width: 25%;
	width: 25%;
	display: flex;
	flex-direction: row;
	flex-wrap: wrap;
	justify-content: space-around;
	align-items: center;
	gap: 20px;
	padding: 20px;
/* 	filter: grayscale(100%); */
	border: 1px solid white;
	background-color: black;
}

.texto {
	width: 80%;
	display: flex;
	flex-direction: row;
	flex-wrap: wrap;
	justify-content: center;
	align-items: center;
	gap: 20px;
	padding: 20px;
	color: rgb(255, 255, 255);
	font-size: 1.2rem;
	margin-bottom: 200px;
	margin-top: none;
}

.text-center {
	text-align: center;
	text-decoration: underline 1px solid white;
	font-size: 2.5rem;
}

@media (max-width: 1580px) {

	.texto {
		width: 60%;
		background-color: rgb(0, 0, 0);
		opacity: 1;
		font-size: 1.2rem;
	}


	.container {
		opacity: 0.8;
	}
}

@media (max-width: 900px) {
	.personal {
		width: 40%;
		margin-bottom: 40px;
	}
}

	.text-center {
		font-size: 1.5rem;
	}

	@media (max-width: 750px) {
	.container {
		width: 100%;
	}


	.texto {
	
	width: 90%;
	font-size: 1rem;
	margin-bottom: 40px;
}	

	.personal {
		width: 80%;
		margin-bottom: 40px;
	}
}


</style>