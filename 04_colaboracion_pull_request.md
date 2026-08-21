# Colaboración profesional con GitHub y Pull Request

En este módulo aprenderás a colaborar en un proyecto de forma organizada, profesional y siguiendo buenas prácticas. La idea es que cada alumno cree su propia carpeta con su nombre y suba el producto final del módulo 03, modificando la landing page que ya desarrollaste.

## Objetivo

Cada estudiante:

- creará una carpeta personal dentro del repositorio del proyecto
- colocará su versión final del proyecto del módulo 03
- trabajará en una rama independiente
- hará commits claros y descriptivos
- abrirá un Pull Request (PR) para que el proyecto pueda revisarse y integrarse correctamente

---

## Objetivo del ejercicio

El proyecto se convertirá en un espacio colaborativo donde cada alumno aporta su diseño personalizado, manteniendo una estructura ordenada y siguiendo estándares profesionales.

La actividad no solo evalúa el proyecto visual, sino también:

- la organización del código
- el uso correcto de Git
- la calidad de los commits
- la claridad del Pull Request
- el respeto de buenas prácticas de trabajo en equipo

---

## Estructura esperada del repositorio

El repositorio principal debe quedar con una estructura similar a esta:

```text
HTML_CSS/
├── 00_indice.md
├── 01_html_basico.md
├── 02_css_basico.md
├── 03_proyecto_final.md
├── 04_colaboracion_pull_request.md
├── README.md
├── alumnos/
│   ├── ana-lopez/
│   │   ├── index.html
│   │   ├── style.css
│   │   └── README.md
│   ├── carlos-ramirez/
│   │   ├── index.html
│   │   ├── style.css
│   │   └── README.md
│   └── ...
└── .gitignore
```

### Reglas importantes

- Cada alumno debe tener su propia carpeta.
- El nombre de la carpeta debe ser claro y consistente, por ejemplo:
  - `ana-lopez`
  - `carlos-ramirez`
  - `maria-gonzalez`
- La carpeta debe contener al menos:
  - `index.html`
  - `style.css`
  - opcionalmente un `README.md` propio

---

## Flujo de trabajo recomendado

### 1. Clonar el repositorio

```bash
git clone <URL-del-repositorio>
cd HTML_CSS
```

### 2. Crear una rama de trabajo

Cada alumno debe crear una rama específica para su trabajo.

```bash
git checkout -b feature/ana-lopez-proyecto-final
```

### Buenas prácticas para nombres de ramas

Usa nombres descriptivos y consistentes:

- `feature/ana-lopez-landing-page`
- `feature/carlos-proyecto-final`
- `fix/ana-ajuste-responsive`

Evita nombres como:

- `rama1`
- `prueba`
- `cambios-finales`

---

### 3. Crear la carpeta personal

Dentro del proyecto, crea una carpeta con tu nombre.

```text
alumnos/
└── ana-lopez/
```

Dentro de esa carpeta coloca los archivos resultantes del módulo 03, por ejemplo:

```text
alumnos/ana-lopez/
├── index.html
├── style.css
└── README.md
```

### 4. Ajustar el proyecto personal

Modifica el proyecto del módulo 03 para que sea más personal. Puedes cambiar:

- nombre del proyecto
- colores
- tipografía
- textos
- sección de contacto
- foto o imagen
- información académica o personal

### 5. Validar antes de subir

Antes de hacer commit, revisa que todo funcione correctamente:

- abre el archivo `index.html` en el navegador
- verifica que no haya errores visuales importantes
- comprueba que el diseño se vea bien en desktop y móvil
- asegúrate de que los enlaces e imágenes funcionen
- confirma que no haya archivos vacíos o código duplicado

---

## Commits profesionales

Todos los cambios deben hacerse con commits claros y significativos.

### Ejemplo de commit correcto

```bash
git add .
git commit -m "feat: agrega landing page personalizada de Ana López"
```

### Ejemplos de mensajes buenos

- `feat: crea estructura inicial de la landing page`
- `style: personaliza paleta de colores y tipografía`
- `fix: corrige diseño responsivo en mobile`
- `docs: agrega README de la carpeta del alumno`

### Evita mensajes vagos como:

- `cambios`
- `actualización`
- `listo`
- `final final`

---

## Subir cambios al repositorio

Cuando tus cambios estén listos, haz push a tu rama:

```bash
git push origin feature/ana-lopez-proyecto-final
```

Si el repositorio es compartido y se usa un fork, también puedes seguir este flujo:

```bash
git remote -v
```

Y luego:

```bash
git push origin feature/ana-lopez-proyecto-final
```

---

## Crear un Pull Request

### Paso 1: abrir PR en GitHub

En el repositorio, busca la opción:

- Compare & pull request
- o New pull request

### Paso 2: seleccionar ramas

Asegúrate de que la rama origen sea tu rama de trabajo y la destino sea la rama principal del proyecto, por ejemplo:

- base: `main`
- compare: `feature/ana-lopez-proyecto-final`

### Paso 3: completar el PR con información clara

El título debe ser profesional y descriptivo.

#### Ejemplo de título

```text
feat: agrega landing page personalizada de Ana López
```

#### Ejemplo de descripción

```md
## Descripción

Se agrega la versión personalizada de la landing page del módulo 03, con cambios en:

- paleta de colores
- contenido textual
- estructura visual
- diseño responsivo

## Archivos incluidos

- alumnos/ana-lopez/index.html
- alumnos/ana-lopez/style.css
- alumnos/ana-lopez/README.md

## Verificación

- revisado visualmente en navegador
- comprobado en vista desktop y mobile
- validado que el formulario y el diseño funcionan correctamente
```

---

## Buenas prácticas para Pull Requests

### Debe incluir

- título claro
- descripción breve y objetiva
- lista de cambios realizados
- referencia a archivos importantes
- validación o prueba realizada

### Evita

- PRs con título genérico como `Cambios`
- descripciones vacías
- subir archivos sin revisar
- incluir archivos innecesarios
- hacer commits muy grandes sin contexto

---

## Checklist de revisión antes del PR

Antes de abrir el pull request, verifica esta lista:

- [ ] La carpeta personal tiene un nombre correcto
- [ ] El proyecto está dentro de `alumnos/<nombre>/`
- [ ] Los archivos fueron modificados y están organizados
- [ ] El `index.html` y `style.css` están completos
- [ ] El proyecto se ve bien en navegador
- [ ] El diseño es responsivo
- [ ] Los commits tienen mensajes claros
- [ ] La rama tiene un nombre profesional
- [ ] La descripción del PR es clara
- [ ] No hay archivos basura o temporales

---

## Ejemplo de estructura final del alumno

```text
alumnos/ana-lopez/
├── index.html
├── style.css
├── README.md
└── assets/
    └── banner.jpg
```

El README de la carpeta puede incluir:

```md
# Proyecto personal de Ana López

## Descripción
Este proyecto fue desarrollado a partir del módulo 03 y personalizado con mi información académica.

## Tecnologías usadas
- HTML
- CSS

## Cómo abrirlo
Abre el archivo `index.html` en tu navegador.
```

---

## Recomendaciones de trabajo en equipo

- nunca trabajes directamente en la rama principal
- usa ramas para cada tarea
- revisa cambios antes de hacer push
- comunica claramente qué modificaste
- si el proyecto es colaborativo, usa comentarios en el PR para explicar decisiones
- responde a comentarios de revisión con respeto y claridad

---

## Regla de oro del trabajo profesional

Un buen proyecto no se trata solo de que se vea bonito, sino de que esté bien organizado, documentado y sea fácil de revisar por otras personas.

---

## Siguiente paso

El objetivo final es que cada alumno:

1. desarrolle su versión del proyecto,
2. la organice dentro de su carpeta personal,
3. envíe sus cambios por una rama,
4. abra un Pull Request profesional,
5. y aprenda a colaborar con su equipo como si fuera un proyecto real.

---

## Reto final

Crea tu propia carpeta con tu nombre y añade tu versión del proyecto final del módulo 03. Luego:

- crea una rama con tu nombre,
- haz tus commits con mensajes claros,
- sube tus archivos,
- y crea un Pull Request con una descripción profesional.

Esto te ayudará a adquirir una práctica real de colaboración en desarrollo web.
