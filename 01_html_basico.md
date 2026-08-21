# HTML básico para principiantes

HTML significa HyperText Markup Language. Se usa para crear la estructura de una página web.

## 1. Estructura mínima de una página

Crea un archivo llamado `index.html` y copia este contenido:

```html
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Mi primera página</title>
  </head>
  <body>
    <h1>Hola, mundo</h1>
    <p>Esta es mi primera página web.</p>
  </body>
</html>
```

### ¿Qué hace cada parte?

- `<!DOCTYPE html>`: indica que el documento es HTML5.
- `<html>`: contenedor principal.
- `<head>`: metadatos, título, configuración.
- `<body>`: todo lo que el usuario ve.
- `<h1>`: encabezado principal.
- `<p>`: párrafo.

### Ejercicio

Cambia el texto para que diga algo sobre ti.

---

## 2. Encabezados y párrafos

```html
<h1>Título principal</h1>
<h2>Subtítulo</h2>
<h3>Sección pequeña</h3>

<p>Este es un párrafo normal.</p>
<p>Otro párrafo con más información.</p>
```

### Importante

Los encabezados van en orden:
- `h1`
- `h2`
- `h3`
- `h4`
- `h5`
- `h6`

No debes saltarte niveles sin necesidad.

---

## 3. Listas

### Lista no ordenada

```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>
```

### Lista ordenada

```html
<ol>
  <li>Estudiar</li>
  <li>Practicar</li>
  <li>Crear proyectos</li>
</ol>
```

### Ejercicio

Haz una lista con tus materias favoritas.

---

## 4. Enlaces e imágenes

### Enlace

```html
<a href="https://www.google.com" target="_blank">Ir a Google</a>
```

### Imagen

```html
<img src="https://via.placeholder.com/300" alt="Imagen de ejemplo" width="300" />
```

### Ejercicio

Crea un enlace a una página con información sobre tu universidad y agrega una imagen.

---

## 5. Semántica básica

HTML moderno usa etiquetas con significado:

```html
<header>
  <h1>Mi sitio</h1>
</header>

<nav>
  <a href="#inicio">Inicio</a>
  <a href="#sobre">Sobre mí</a>
  <a href="#contacto">Contacto</a>
</nav>

<main>
  <section>
    <h2>Sobre mí</h2>
    <p>Soy estudiante de licenciatura.</p>
  </section>
</main>

<footer>
  <p>Todos los derechos reservados.</p>
</footer>
```

### ¿Por qué es importante?

Porque mejora la organización del contenido y ayuda a accesibilidad y SEO.

---

## 6. Formulario básico

```html
<form>
  <label for="nombre">Nombre:</label>
  <input type="text" id="nombre" name="nombre" />

  <br /><br />

  <label for="correo">Correo:</label>
  <input type="email" id="correo" name="correo" />

  <br /><br />

  <button type="submit">Enviar</button>
</form>
```

### Elementos usados

- `label`: describe el campo
- `input`: captura información
- `button`: botón de acción

### Ejercicio

Crea un formulario con nombre, carrera y botón de enviar.

---

## 7. Tabla simple

```html
<table border="1">
  <tr>
    <th>Materia</th>
    <th>Horario</th>
  </tr>
  <tr>
    <td>Programación web</td>
    <td>Martes 9:00</td>
  </tr>
  <tr>
    <td>Algoritmos</td>
    <td>Jueves 11:00</td>
  </tr>
</table>
```

---

## 8. Proyecto mini 1: carta personal

Copia este ejemplo y guárdalo como `perfil.html`:

```html
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Perfil personal</title>
  </head>
  <body>
    <header>
      <h1>Mi perfil</h1>
    </header>

    <main>
      <section>
        <h2>Datos</h2>
        <p>Nombre: Ana López</p>
        <p>Carrera: Ingeniería en Sistemas</p>
      </section>

      <section>
        <h2>Hobbies</h2>
        <ul>
          <li>Leer</li>
          <li>Programar</li>
          <li>Escuchar música</li>
        </ul>
      </section>

      <section>
        <h2>Contacto</h2>
        <a href="mailto:ana@email.com">Enviar correo</a>
      </section>
    </main>
  </body>
</html>
```

### Tarea

Cámbialo con tus datos reales.

---

## 9. Resumen rápido

En HTML aprendiste:
- cómo crear la estructura de una página
- cómo usar títulos, párrafos y listas
- cómo agregar enlaces e imágenes
- cómo crear formularios y tablas
- cómo organizar contenido con etiquetas semánticas

## Siguiente paso

Ahora ve a [02_css_basico.md](02_css_basico.md) para aprender a dar estilo a esta página.
