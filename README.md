
# Plan de Natanael
Bienvenido a mi proyecto de profesor de informática 😎

<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Plan Docente - Natanael Torres</title>
    <link rel="stylesheet" href="style.css">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet">
</head>
<body>
    <header>
        <h1><i class="fas fa-laptop-code"></i> Mi Plan como futuro Profesor de Informática</h1>
        <p>Natanael Torres | 20 años | Ingeniero de Sistemas (Graduado en Tecnologia en Desarrollo de Software)</p>
    </header>

    <main>
        <div class="buttons">
            <button onclick="showSection('propósito')"><i class="fas fa-bullseye"></i> Propósito</button>
            <button onclick="showSection('aprendizaje')"><i class="fas fa-book"></i> Qué van a aprender</button>
            <button onclick="showSection('clases')"><i class="fas fa-chalkboard-teacher"></i> Cómo serán las clases</button>
            <button onclick="showSection('comunicacion')"><i class="fas fa-comments"></i> Comunicación</button>
            <button onclick="showSection('reconocimientos')"><i class="fas fa-award"></i> Reconocimientos</button>
            <button onclick="showSection('actividades')"><i class="fas fa-tasks"></i> Actividades</button>
        </div>

        <div class="section" id="propósito">
            <h2><i class="fas fa-bullseye"></i> 1. Propósito</h2>
            <p>Enseñar informática de forma fácil, divertida y útil para que los estudiantes puedan implementar en su vida diaria y en un futuro.</p>
        </div>

        <div class="section" id="aprendizaje">
            <h2><i class="fas fa-book"></i> 2. Qué van a aprender</h2>
            <ul>
                <li>Microsoft Word → Documentos</li>
                <li>Microsoft Excel → Tablas y fórmulas</li>
                <li>Microsoft PowerPoint → Presentaciones</li>
                <li>Programación básica → Último periodo</li>
            </ul>
        </div>

        <div class="section" id="clases">
            <h2><i class="fas fa-chalkboard-teacher"></i> 3. Cómo serán las clases</h2>
            <ul>
                <li>Prácticas y fáciles</li>
                <li>Actividades divertidas</li>
                <li>Talleres para practicar</li>
                <li>Resolver dudas sin miedo</li>
            </ul>
        </div>

        <div class="section" id="comunicacion">
            <h2><i class="fas fa-comments"></i> 4. Comunicación con acudientes</h2>
            <p>Grupo de WhatsApp por curso (solo acudientes). Allí se envían avisos, tareas y noticias.</p>
        </div>

        <div class="section" id="reconocimientos">
            <h2><i class="fas fa-award"></i> 5. Reconocimientos</h2>
            <ul>
                <li>Mejor estudiante será el "Alumno Feliz"</li>
                <li>Foto enviada al acudiente</li>
                <li>Calendario de cumpleaños</li>
            </ul>
        </div>

        <div class="section" id="actividades">
            <h2><i class="fas fa-tasks"></i> 6. Actividades especiales</h2>
            <ul>
                <li>Retos semanales</li>
                <li>Concursos de presentaciones</li>
                <li>Trabajos en equipo</li>
            </ul>
        </div>
    </main>

    <footer>
        <p>&copy; 2025 Natanael Torres</p>
    </footer>

    <script>
        const sections = document.querySelectorAll('.section');
        function showSection(id) {
            sections.forEach(sec => {
                sec.style.display = 'none';
                sec.classList.remove('fadeIn');
            });
            const el = document.getElementById(id);
            el.style.display = 'block';
            setTimeout(() => el.classList.add('fadeIn'), 10);
        }
        showSection('propósito');
    </script>

  Bienvenido al Plan de Natanael

  <section id="descargar-pdf">
    <h2><i class="fas fa-file-pdf"></i> Proyecto Completo</h2>
    <a href="Plan Docente de Natanael Torres.pdf" download class="pdf-button">
        <i class="fas fa-download"></i> Descargue el archivo (Plan de Natanael)
    </a>
</section>

</div>

    </a>
</section>

