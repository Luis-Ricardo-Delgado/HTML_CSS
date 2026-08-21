# Proyecto final: landing page simple

En este ejercicio combinarás HTML y CSS para crear una página web funcional y visualmente agradable.

## Objetivo

Construir una página de presentación para una carrera, un proyecto escolar o una persona.

---

## Paso 1: crea la estructura HTML

Guarda esto como `index.html`:

```html
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Proyecto final</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <header class="hero">
      <nav class="nav">
        <div class="logo">MiProyecto</div>
        <div class="menu">
          <a href="#inicio">Inicio</a>
          <a href="#sobre">Sobre</a>
          <a href="#contacto">Contacto</a>
        </div>
      </nav>

      <section class="hero-content" id="inicio">
        <div>
          <p class="etiqueta">Licenciatura en tecnologías</p>
          <h1>Diseño y desarrollo web</h1>
          <p>
            Aprendo a crear páginas modernas con HTML y CSS para comunicar ideas de forma clara.
          </p>
          <button class="boton">Ver más</button>
        </div>

        <div class="imagen-box">
          <img src="https://via.placeholder.com/400x300" alt="Imagen de ejemplo" />
        </div>
      </section>
    </header>

    <main>
      <section class="seccion" id="sobre">
        <h2>¿Qué aprenderé?</h2>
        <div class="cards">
          <article class="card">
            <h3>HTML</h3>
            <p>Estructura del contenido y semántica.</p>
          </article>
          <article class="card">
            <h3>CSS</h3>
            <p>Diseño visual, colores, espaciado y responsividad.</p>
          </article>
          <article class="card">
            <h3>Práctica</h3>
            <p>Construcción de proyectos reales y ejercicios.</p>
          </article>
        </div>
      </section>

      <section class="seccion contacto" id="contacto">
        <h2>Contacto</h2>
        <form class="formulario">
          <input type="text" placeholder="Tu nombre" />
          <input type="email" placeholder="Tu correo" />
          <button type="submit" class="boton">Enviar</button>
        </form>
      </section>
    </main>
  </body>
</html>
```

---

## Paso 2: crea el estilo CSS

Guarda esto como `style.css`:

```css
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #f5f7fb;
  color: #1f2937;
}

.hero {
  background: linear-gradient(135deg, #1d4ed8, #60a5fa);
  color: white;
  padding: 20px 5%;
}

.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 40px;
}

.logo {
  font-size: 1.5rem;
  font-weight: bold;
}

.menu {
  display: flex;
  gap: 20px;
}

.menu a {
  color: white;
  text-decoration: none;
}

.hero-content {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 30px;
  padding: 30px 0;
}

.etiqueta {
  text-transform: uppercase;
  letter-spacing: 2px;
  font-size: 0.8rem;
  opacity: 0.9;
}

.hero-content h1 {
  font-size: 3rem;
  margin: 10px 0;
}

.hero-content p {
  font-size: 1.1rem;
  line-height: 1.6;
}

.imagen-box img {
  width: 100%;
  max-width: 400px;
  border-radius: 15px;
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
}

.seccion {
  padding: 60px 5%;
}

.cards {
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
  margin-top: 20px;
}

.card {
  background: white;
  padding: 25px;
  border-radius: 12px;
  flex: 1 1 220px;
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.08);
}

.contacto {
  background: #e0f2fe;
}

.formulario {
  display: flex;
  flex-wrap: wrap;
  gap: 15px;
  max-width: 700px;
}

.formulario input {
  flex: 1 1 220px;
  padding: 12px 14px;
  border: 1px solid #cbd5e1;
  border-radius: 8px;
}

.boton {
  background: #f59e0b;
  color: white;
  border: none;
  padding: 12px 22px;
  border-radius: 8px;
  cursor: pointer;
  font-weight: bold;
}

.boton:hover {
  background: #d97706;
}

@media (max-width: 700px) {
  .nav,
  .hero-content {
    flex-direction: column;
    align-items: flex-start;
  }

  .menu {
    flex-direction: column;
    gap: 10px;
  }

  .hero-content h1 {
    font-size: 2.2rem;
  }
}
```

---

## Paso 3: abre la página

Abre `index.html` en tu navegador. Debes ver una página con:
- encabezado azul
- menú de navegación
- imagen a la derecha
- tarjetas de información
- formulario de contacto

---

## Paso 4: prueba tú mismo

Modifica lo siguiente:
- cambia el texto del título
- cambia los colores del fondo
- cambia el texto del botón
- cambia el nombre de la universidad o carrera
- agrega otro bloque de contenido

---

## Reto final

Haz una versión personalizada para:
- tu universidad
- tu carrera
- un proyecto escolar
- una página personal

La idea es que la página se vea diferente, pero con la misma estructura.

---

## Resumen del curso

Con este curso aprendiste:
- a estructurar una página con HTML
- a dar estilo con CSS
- a crear secciones, botones, formularios y tarjetas
- a usar flexbox y media queries
- a construir un proyecto visual simple y práctico

## Siguiente paso

Ahora puedes practicar creando:
- una página personal
- una tarjeta de presentación
- una página para una empresa o club escolar
- una galería de imágenes

¡La práctica es la clave!
