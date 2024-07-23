<script setup>

</script>

<template>

	<div class="container">

			<img src="../../public/personal.jpg" class="personal">

		<div class="texto">
			<h1 class="text-center">Sobre mi</h1>
			<p>1- Título
				Escribe un título que atrape, que haga que la persona que lo ha visto quiera seguir leyendo y no pase
				desapercibido. A su vez, acompáñalo con la parte visual. Escoge un estilo, tamaño y color de tipografía que se
				ajuste a tu empresa.

				Escoge una frase que te defina.

				2- Desarrolla tu propuesta de valor
				Una vez seleccionado el título, que capta la atención de los usuarios, ha llegado la hora de desarrollar tu
				propuesta de valor.

				Saca provecho a los puntos de dolor de tu target e indica la solución que tienes para ellos. ¿Cuál es tu misión?

				Muestra quién eres, a lo que te dedicas, lo que ofreces, qué beneficios pueden conseguir contigo y a quienes
				ayudas.

				Puedes escribir algo como:

				Mi nombre es… y soy… (a qué te dedicas)
				Mi misión es ayudar a … a tener… para…
				¡Qué te parece! ¿Hablamos?</p>
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
	gap: 20px;
	opacity: 0.8;

}

.personal {
	width: 25%;
	display: flex;
	flex-direction: row;
	flex-wrap: wrap;
	justify-content: space-around;
	align-items: center;
	gap: 20px;
	padding: 20px;
	filter: grayscale(100%);
	border: 1px solid white;
}

.text-center {

	text-align: center;
	text-decoration: underline 1px solid white;
	font-size: 2.5rem;
}

.texto {
	width: 80%;
	display: flex;
	flex-direction: row;
	flex-wrap: wrap;
	justify-content: space-around;
	align-items: center;
	gap: 20px;
	padding: 20px;
	color: rgb(255, 255, 255);
	font-size: 1.1rem;
	margin-bottom: 200px; 
}

</style>