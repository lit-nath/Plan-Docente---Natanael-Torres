<!DOCTYPE html>
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
        <p>Natanael Torres | 20 años | Graduado en Desarrollo de Software</p>
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

<section id="descargar-pdf">
    <h2><i class="fas fa-file-pdf"></i> Proyecto Completo</h2>
    <a href="Plan Docente de Natanael Torres.pdf" download class="pdf-button">
        <i class="fas fa-download"></i> Descargue el archivo (Plan de Natanael)
    </a>
</section>

/* Fondo animado degradado azul */
body {
    font-family: 'Arial', sans-serif;
    margin: 0;
    padding: 0;
    background: linear-gradient(-45deg, #0b3d91, #1e90ff, #00bfff, #87cefa);
    background-size: 400% 400%;
    animation: gradientBG 15s ease infinite;
    color: #fff;
}

@keyframes gradientBG {
    0% {background-position: 0% 50%;}
    50% {background-position: 100% 50%;}
    100% {background-position: 0% 50%;}
}

/* Header */
header {
    text-align: center;
    padding: 30px 20px;
    background: rgba(0,0,0,0.2);
    box-shadow: 0 2px 10px rgba(0,0,0,0.3);
}

header h1 {
    margin: 0;
    font-size: 28px;
}

header p {
    margin: 5px 0 0;
    font-size: 16px;
}

/* Botones */
.buttons {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    margin: 20px 0;
}

.buttons button {
    background-color: rgba(255,255,255,0.2);
    border: none;
    color: #fff;
    padding: 12px 20px;
    margin: 5px;
    border-radius: 25px;
    cursor: pointer;
    transition: all 0.3s;
    font-size: 14px;
}

.buttons button:hover {
    background-color: rgba(255,255,255,0.5);
    transform: scale(1.05);
}

/* Secciones */
.section {
    display: none;
    max-width: 800px;
    margin: 0 auto 30px;
    padding: 20px;
    background: rgba(0,0,0,0.2);
    border-radius: 15px;
    box-shadow: 0 4px 10px rgba(0,0,0,0.3);
    opacity: 0;
    transition: opacity 0.7s ease;
}

.section.fadeIn {
    opacity: 1;
}

.section h2 {
    margin-top: 0;
    font-size: 22px;
    border-bottom: 2px solid #fff;
    padding-bottom: 5px;
}

.section ul {
    padding-left: 20px;
}

/* Footer */
footer {
    text-align: center;
    padding: 20px;
    background: rgba(0,0,0,0.2);
    font-size: 14px;
}

/* Iconos */
i {
    margin-right: 8px;
}


.pdf-button {
    display: inline-block;
    background-color: #ff4c4c;
    color: white;
    padding: 12px 20px;
    border-radius: 25px;
    text-decoration: none;
    font-weight: bold;
    margin: 10px 0;
    transition: all 0.3s;
}

.pdf-button:hover {
    background-color: #ff1a1a;
    transform: scale(1.05);
}

/* Estilo para el iframe */
iframe {
    border: 2px solid rgba(255,255,255,0.5);
    border-radius: 15px;
    margin-top: 15px;
}


.pdf-button {
    display: inline-block;
    background-color: #180337;
    color: white;
    padding: 15px 25px;
    border-radius: 30px;
    text-decoration: none;
    font-weight: bold;
    font-size: 16px;
    margin-top: 15px;
    transition: all 0.3s;
}

.pdf-button:hover {
    background-color: #1aa0ff;
    transform: scale(1.05);
    box-shadow: 0 5px 15px rgba(0,0,0,0.3);
}

</body>
</html>
