<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fundación de Abuelitos</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            text-align: center;
        }
        header {
            background: #333;
            color: white;
            padding: 15px;
            text-align: center;
        }
        nav ul {
            list-style: none;
            padding: 0;
        }
        nav ul li {
            display: inline;
            margin: 0 10px;
        }
        nav ul li a {
            color: white;
            text-decoration: none;
            font-size: 18px;
        }
        .seccion {
            padding: 20px;
            display: none;
        }
        .seccion:first-of-type {
            display: block;
        }
        .boton {
            display: inline-block;
            padding: 10px 20px;
            margin: 10px;
            background: #007BFF;
            color: white;
            text-decoration: none;
            border-radius: 5px;
        }
        .boton:hover {
            background: #0056b3;
        }
    </style>
    <script>
        function mostrarSeccion(id) {
            let secciones = document.querySelectorAll('.seccion');
            secciones.forEach(seccion => {
                seccion.style.display = 'none';
            });
            document.getElementById(id).style.display = 'block';
        }
    </script>
</head>
<body>
    <header>
        <h1>Fundación de Abuelitos</h1>
        <nav>
            <ul>
                <li><a href="#inicio" onclick="mostrarSeccion('inicio')">Inicio</a></li>
                <li><a href="#nosotros" onclick="mostrarSeccion('nosotros')">Nosotros</a></li>
                <li><a href="#ayudanos" onclick="mostrarSeccion('ayudanos')">Ayúdanos</a></li>
                <li><a href="#contacto" onclick="mostrarSeccion('contacto')">Contacto</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section id="inicio" class="seccion">
            <h2>Bienvenidos a la Fundación</h2>
            <p>Somos una organización dedicada al bienestar de los adultos mayores, brindándoles apoyo y compañía.</p>
            <blockquote>"Ayudar a los abuelitos es devolverles el amor que nos dieron."</blockquote>
        </section>
        <section id="nosotros" class="seccion oculto">
            <h2>Nuestra Historia</h2>
            <p>La fundación fue creada con el propósito de mejorar la calidad de vida de los adultos mayores...</p>
            <p><strong>Ubicación:</strong> [Dirección aquí]</p>
            <p><strong>Tiempo de actividad:</strong> [Años de la fundación]</p>
        </section>
        <section id="ayudanos" class="seccion oculto">
            <h2>Cómo Ayudar</h2>
            <p>Puedes colaborar con nuestra causa a través de donaciones monetarias o en especie.</p>
            <a href="[LINK FORMULARIO DINERO]" class="boton">Donar Dinero</a>
            <a href="[LINK FORMULARIO ESPECIE]" class="boton">Donar en Especie</a>
        </section>
        <section id="contacto" class="seccion oculto">
            <h2>Contacto</h2>
            <p><strong>Teléfono:</strong> [Número de contacto]</p>
            <p><strong>Personas a cargo:</strong> [Nombres aquí]</p>
        </section>
    </main>
</body>
</html>

