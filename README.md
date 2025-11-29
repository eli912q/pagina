<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Bootstrap uso medio</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
  <style>
    .hero {
      padding: 48px;
      background: linear-gradient(180deg, #eef6ff, #fff);
    }

    .speaker-img{
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 8px;
    }
  </style>
</head>
<body>

  <header class="navbar navbar-expand-lg navbar-dark bg-primary">
    <div class="container">
      <a class="navbar-brand" href="#">IA Challenge Latam</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navMain">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navMain">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link" href="#speakers">Conecta </a></li>
          <li class="nav-item"><a class="nav-link" href="#schedule">Programa</a></li>
          <li class="nav-item"><a class="nav-link" href="#gallery">Galería</a></li>
        </ul>
      </div>
    </div>
  </header>

  <!-- HERO -->
  <section class="hero">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-12 col-md-7">
          <h1 class="display-5">Hackathon2026</h1>
          <p class="lead">Desafía el Futuro con Innovación</p>
          <button class="btn btn-lg btn-primary" data-bs-toggle="modal" data-bs-target="#ticketModal">¡Inscribe a tu equipo ahora!</button>
        </div>
        <div class="col-12 col-md-5">
          <img src="https://cdn.forbes.com.mx/2024/01/tecnologias-de-la-informacion-1024x661.png" alt="Evento" class="img-fluid rounded">
        </div>
      </div>
    </div>
  </section>

  <!-- SPEAKERS: anidado con row-cols y card dentro de cada col -->
  <section id="speakers" class="py-5">
    <div class="container">
      <h2 class="mb-4">Jueces</h2>

      
      <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3 ">
        <!-- Ejemplo de una card de speaker (el grupo debe duplicar/editar) -->
        <div class="col">
          <article class="card h-100">
            <img src="https://cdn-3.expansion.mx/dims4/default/d033815/2147483647/strip/true/crop/1365x768+0+0/resize/1800x1013!/format/webp/quality/80/?url=https%3A%2F%2Fcdn-3.expansion.mx%2Fed%2F18%2F979c70fa4b81871b5a1e4fa98100%2Frecursos-humanos-demanda-cada-vez-mas-tecnologia-en-su-estrategia.jpeg" class="speaker-img card-img-top" alt="">
            <div class="card-body d-flex flex-column">
              <h5 class="card-title">Jorge Domínguez</h5>
              <p class="card-text muted">Lead Product Manager 
                <br>Generalist UX Designer
              </p>
              <div class="mt-auto">
                <!-- tooltip: atributos para inicializar -->
                <button class="btn btn-outline-primary btn-sm" title="Ver bio">Bio</button>
              </div>
            </div>
          </article>
        </div>



        <div class="col">
          <article class="card h-100">
            <img src="https://www.shutterstock.com/image-photo/ai-expert-showcasing-cutting-edge-260nw-2503872335.jpg" class="speaker-img card-img-top" alt="">
            <div class="card-body d-flex flex-column">
              <h5 class="card-title">Julia Rodríguez </h5>
              <p class="card-text muted">Experta en diseño, aplicación y análisis de modelos de IA</p>
              <div class="mt-auto">
                <!-- tooltip: atributos para inicializar -->
                <button class="btn btn-outline-primary btn-sm" title="Ver bio">Bio</button>
              </div>
            </div>
          </article>
        </div>

        <div class="col">
          <article class="card h-100">
            <img src="https://www.shutterstock.com/image-photo/man-speaking-tech-expo-exploring-600nw-2498849247.jpg" class="speaker-img card-img-top" alt="">
            <div class="card-body d-flex flex-column">
              <h5 class="card-title">Daniel Lozada</h5>
              <p class="card-text muted">Experto en Arquitectura Cloud e Ingeniería Ambiental</p>
              <div class="mt-auto">
                <!-- tooltip: atributos para inicializar -->
                <button class="btn btn-outline-primary btn-sm" title="Ver bio">Bio</button>
              </div>
            </div>
          </article>
        </div>


        
    
      </div>
    </div>
  </section>

  <!-- SCHEDULE: grid anidado por día y por track -->
  <section id="schedule" class="py-5 bg-light">
    <div class="container">
      <h2 class="mb-4">Programa</h2>

      <!-- Estructura: row con 2 columnas (día 1 / día 2). En cada col anidar lista de tracks -->
      <div class="row g-3">
        <div class="col-12 col-md-6">
          <div class="panel p-3">
            <h5>Día 1</h5>
            <div class="row g-2">
              <!-- cada fila representa una sesión: hora + title -->
              <div class="col-3">09:00</div>
              <div class="col-9">
Bienestar Humano y Salud Global
<br>

¿Cómo puede la IA mejorar la calidad de vida, 
optimizar el acceso a la salud o prevenir enfermedades a nivel mundial? 
Desde la equidad en el acceso hasta el apoyo emocional, tu innovación puede marcar la diferencia.
</div>
              <!-- Añadir más sesiones con anidación en grid -->
            </div>
          </div>
        </div>

        <div class="col-12 col-md-6">
          <div class="panel p-3">
            <h5>Día 2</h5>
            <div class="row g-2">
              <div class="col-3">09:00</div>
              <div class="col-9">
Educación y Futuro del Trabajo
<br>

Revoluciona el aprendizaje, la enseñanza y el mundo laboral con IA. 
Piensa en plataformas personalizadas, herramientas para el trabajo remoto o soluciones
 para la reconversión profesional. El futuro del trabajo está en tus manos.
a</div>
              <!-- Completar -->
            </div>
          </div>
        </div>
      </div>

    </div>
  </section>

  <!-- GALLERY (carousel) -->
  <section id="gallery" class="py-5">
    <div class="container">
      <h2 class="mb-4">Galería</h2>

      <div id="eventCarousel" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-inner">
          <div class="carousel-item active">
            <img src="https://img.freepik.com/foto-gratis/grupo-jovenes-gafas-vr-haciendo-experimentos-robotica-laboratorio-robot-sobre-mesa_1268-24393.jpg?semt=ais_hybrid&w=740&q=80" class="d-block w-100" alt="...">
          </div>
          <div class="carousel-item">
            <img src="https://img.freepik.com/foto-gratis/tecnologia-integrada-vida-cotidiana_23-2151887043.jpg?semt=ais_hybrid&w=740&q=80" class="d-block w-100" alt="...">
          </div>
          <!-- Añadir 1–2 slides más -->
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#eventCarousel" data-bs-slide="prev">
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Anterior</span>
        </button>

        <button class="carousel-control-next" type="button" data-bs-target="#eventCarousel" data-bs-slide="next">
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Siguiente</span>
        </button>
       
      </div>
    </div>
  </section>

 

  <!-- Bootstrap JS bundle -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>

  <script>
    // Inicializar tooltips (grupo debe llamarlo una vez)
    document.addEventListener('DOMContentLoaded', function () {
      var t = [].slice.call(document.querySelectorAll('[data-bs-toggle="tooltip"]'));
      t.forEach(function (el) { new bootstrap.Tooltip(el); });
    });
  </script>
</body>
</html>
# pagina
pagina
