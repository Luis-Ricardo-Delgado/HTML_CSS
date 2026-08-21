# CSS básico para principiantes

CSS significa Cascading Style Sheets. Se usa para dar estilo a una página HTML.

## 1. ¿Qué es CSS?

HTML estructura el contenido. CSS decide:
- color
- tamaño
- fuente
- fondo
- posición
- espaciado

---

## 2. Primera forma de usar CSS

Crea un archivo llamado `style.css` y agrega este contenido:

```css
body {
  font-family: Arial, sans-serif;
  background-color: #f4f4f4;
  color: #333;
}

h1 {
  color: #0b5fff;
  text-align: center;
}

p {
  font-size: 18px;
  line-height: 1.6;
}
```

Ahora enlázalo desde el archivo HTML:

```html
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Mi página con CSS</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <h1>Hola, soy estudiante</h1>
    <p>Estoy aprendiendo HTML y CSS.</p>
  </body>
</html>
```

### ¿Qué ocurrió?

- `body` cambia el fondo y la fuente general.
- `h1` cambia el color y la alineación.
- `p` cambia el tamaño y la separación entre líneas.

---

## 3. Selectores básicos

### Selector de etiqueta

```css
p {
  color: green;
}
```

### Selector de clase

```html
<p class="destacado">Texto importante</p>
```

```css
.destacado {
  color: red;
  font-weight: bold;
}
```

### Selector de id

```html
<p id="mensaje">Este es un mensaje especial</p>
```

```css
#mensaje {
  background-color: yellow;
  padding: 10px;
}
```

### Ejercicio

Haz un párrafo destacado y uno con fondo amarillo.

---

## 4. Colores y fuentes

```css
body {
  background-color: #eef6ff;
  color: #222;
  font-family: "Segoe UI", Tahoma, sans-serif;
}

h2 {
  color: #b10b4a;
}
```

### Colores comunes

- rojo: `red`
- azul: `blue`
- verde: `green`
- negro: `black`
- blanco: `white`

Puedes usar colores hexadecimales como:
- `#ff0000`
- `#00ff88`
- `#1e3a8a`

---

## 5. Modelo de caja (Box Model)

Cada elemento en HTML se ve como una caja.

```css
.caja {
  width: 300px;
  height: 150px;
  background: #dff0ff;
  padding: 20px;
  border: 2px solid #1d4ed8;
  margin: 30px;
}
```

### Partes de la caja

- `width`: ancho
- `height`: alto
- `padding`: espacio interno
- `border`: borde
- `margin`: espacio externo

### Ejemplo HTML

```html
<div class="caja">
  Este es un bloque con estilo.
</div>
```

---

## 6. Alineación y texto

```css
.texto-central {
  text-align: center;
}

.texto-subrayado {
  text-decoration: underline;
}
```

### Ejemplo

```html
<p class="texto-central">Texto centrado</p>
<p class="texto-subrayado">Texto subrayado</p>
```

---

## 7. Botones simples

```html
<button class="boton">Enviar</button>
```

```css
.boton {
  background-color: #2563eb;
  color: white;
  border: none;
  padding: 12px 24px;
  border-radius: 8px;
  cursor: pointer;
}

.boton:hover {
  background-color: #1d4ed8;
}
```

### Pseudoclase hover

`:hover` cambia el estilo cuando el mouse pasa sobre el elemento.

---

## 8. Flexbox básico

Flexbox permite organizar elementos en filas o columnas.

### HTML

```html
<div class="contenedor">
  <div class="caja1">A</div>
  <div class="caja2">B</div>
  <div class="caja3">C</div>
</div>
```

### CSS

```css
.contenedor {
  display: flex;
  justify-content: space-between;
  gap: 20px;
}

.caja1, .caja2, .caja3 {
  width: 100px;
  height: 100px;
  background: #93c5fd;
  display: flex;
  align-items: center;
  justify-content: center;
}
```

### ¿Qué hace?

- `display: flex;` activa el layout flexible
- `justify-content: space-between;` separa los elementos
- `gap` agrega espacio entre elementos

---

## 9. Diseño responsivo con media queries

```css
body {
  background-color: white;
}

@media (max-width: 600px) {
  body {
    background-color: #e0f2fe;
  }

  .contenedor {
    flex-direction: column;
  }
}
```

Esto permite adaptar la página a pantallas pequeñas, como celulares.

---

## 10. Proyecto mini 2: tarjeta de estudiante

Crea `index.html` con este contenido:

```html
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Tarjeta</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="tarjeta">
      <h2>Ana López</h2>
      <p>Estudiante de ingeniería</p>
      <button class="boton">Contactar</button>
    </div>
  </body>
</html>
```

Y `style.css`:

```css
body {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  background: linear-gradient(to right, #dbeafe, #f0fdf4);
  font-family: Arial, sans-serif;
}

.tarjeta {
  background: white;
  padding: 30px;
  border-radius: 15px;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
  text-align: center;
}

.boton {
  background: #2563eb;
  color: white;
  border: none;
  padding: 10px 20px;
  border-radius: 8px;
  cursor: pointer;
}
```

### Tarea

Cambia el nombre, el color y el texto del botón.

---

## 11. Resumen rápido

En CSS aprendiste:
- a conectar archivos CSS
- selectores básicos
- colores, tipografías y fondo
- box model
- hover, flexbox y diseño responsivo

## Siguiente paso

Ve a [03_proyecto_final.md](03_proyecto_final.md) para crear una página completa.
