<!DOCTYPE html>
<html lang="es">
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Mi Sitio Web</title>
	<link rel="stylesheet" href="estilos.css">
</head>

<body>

<header>
	<nav>
		<!-- Enlaces internos -->
		<a href="contacto.html">Contacto</a>
		<a href="./Pagina/info.html">Info</a>

		<!-- Anclas -->
		<a href="#seccion2">Ir a sección 2</a>
		<a href="#formulario">Ir a formulario</a>

		<!-- Enlace externo -->
		<a href="https://google.com" target="_blank" rel="noopener">
			Ir a Google
		</a>
	</nav>
</header>

<main>

	<!-- Sección destino del ancla -->
	<h2 id="seccion2">Sección 2</h2>

	<!-- ================= IMÁGENES ================= -->
	<h2>Imagenes</h2>

	<!-- Imagen básica -->
		<img src="imagenes/informatica.jpg" alt="descripcion">

	<br>
	<br>

	<!-- Imagen con tamaño -->
	<img src="imagenes/miniatura.jpg" width="450" height="300" alt="Logo empresa">

	<br>
	<br>

	<!-- Imagen responsive -->
	<img src="imagenes/logo.jpg" style="width:100%; max-width:800px; height:auto;" alt="Banner">

	<br>
	<br>

	<!-- Imagen como enlace -->
	<a href="detalle.html">
		<img src="imagenes/miniatura.jpg" width="450" alt="Ver detalle">
	</a>

	<br><br>

	<!-- Otra imagen adaptable -->
	<img src="imagenes/Torres.avif" style="width:50%; height:auto;" alt="Imagen adaptable">

	<hr>
     
	<!-- ================= AUDIO ================= -->
	<h2>audio</h2>

	<!-- audio con controles visibles -->
	<audio controls>
		<source src="audio/imposible.mp3" type="audio/mpeg">
		<source src="audio/melodia.ogg" type="audio/ogg">
		Tu navegador no soporta audio html5.
	</audio>
	
	<!-- Audio al abrir/actualizar la página -->
	 <audio autoplay loop>
		<source src="audio/fondo.mp3" type="audio/mpeg">
	 </audio>


	<!-- Silenciado por defecto (buena práctica) -->
	<audio controls autoplay muted>
		<source src="audio/intro.mp3" type="audio/mpeg">
	</audio>

	<!-- Audio con preload -->
	 <audio controls preload="auto">
		<source src="audio/podcast.mp3" type="audio/mpeg">
	 </audio>

	<hr>

	<!-- ================= VIDEO================ -->
	 <h2>Video</h2>
	 <!-- Video básico con controles -->
	  <video width="640" height="360" controls>
		<source src="video/presentacion.mp4" type="video/mp4">
		<source src="video/presentacion.mp4" type="video/webm">
		Tu navegador no soporta video HTML5.
	  </video>

	  <!-- Video con múltiples atributos -->
	   <video width="800" height="450"
	   controls
	   autoplay
	   muted
	   loop
	   poster="miniatura.jpg"
	   preload="metadata">
	<source src="video/intro.mp4"
	type="video/mp4">
	</video>

	<!-- Video responsive con CSS -->
	 <video style="width:100%; max: width 900px;"
	 controls poster="cover.jpg">
	<source src="video/goku.mp4" type="video/mp4">
	</video> 
	

	<!-- ================= TABLA ================= -->
	<h2>Tabla</h2>

	<table border="1" cellpadding="8" cellspacing="0">
		<thead>
			<tr>
				<th>Nombre</th>
				<th>Apellido</th>
				<th>Correo</th>
			</tr>
		</thead>

		<tbody>
			<tr>
				<td>Ana</td>
				<td>López</td>
				<td>ana@email.com</td>
			</tr>

			<tr>
				<td colspan="2">Fusión de columnas</td>
				<td>ejemplo@mail.com</td>
			</tr>
		</tbody>

		<tfoot>
			<tr>
				<td colspan="3">Total: 2 registros</td>
			</tr>
		</tfoot>
	</table>

	<hr>

	<!-- ================= FORMULARIO ================= -->
	<section id="formulario">
		<h2>Formulario de Registro</h2>

		<form action="procesar.php" method="post">

			<label for="nombre">Nombre:</label><br>
			<input type="text" id="nombre" name="nombre" placeholder="Tu nombre" required>
			<br><br>

			<label for="email">Correo:</label><br>
			<input type="email" id="email" name="email">
			<br><br>

			<label for="pais">País:</label><br>
			<select id="pais" name="pais">
				<option value="gt">Guatemala</option>
				<option value="mx">México</option>
			</select>
			<br><br>

			<label>
				<input type="checkbox" name="acepto" required>
				Acepto términos
			</label>
			<br><br>

			<button type="submit">Enviar</button>

		</form>
	</section>

</main>

<footer>
	<p> 2026 Mi Sitio Web</p>
</footer>

</body>
</html>
