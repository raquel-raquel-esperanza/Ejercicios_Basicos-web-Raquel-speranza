# 🌐 Página Web con HTML5 y CSS3

**Actividad Evaluada — Desarrollo Web Básico**
**Tipo de actividad:** Evaluada

---

## 🎯 Propósito de Aplicación

Construir una página web completa con temática de **tecnología** aplicando:

- Estructura semántica de HTML5
- Elementos de contenido correctamente organizados
- Un formulario funcional
- Estilos visuales básicos con CSS3

---

## 📁 Estructura del Proyecto

```
proyecto-web/
├── index.html
└── style.css
```

---

## 🧱 Estructura HTML5 (`index.html`)

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Tecnología Web</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>

  <!-- Encabezado principal -->
  <header>
    <h1>🌐 Mundo Tech</h1>
    <nav>
      <ul>
        <li><a href="#inicio">Inicio</a></li>
        <li><a href="#articulos">Artículos</a></li>
        <li><a href="#contacto">Contacto</a></li>
      </ul>
    </nav>
  </header>

  <!-- Contenido principal -->
  <main>

    <!-- Sección de bienvenida -->
    <section id="inicio">
      <h2>Bienvenidos al futuro digital</h2>
      <p>
        Explora las últimas tendencias en tecnología: inteligencia artificial,
        desarrollo web, ciberseguridad y mucho más.
      </p>
    </section>

    <!-- Sección de artículos -->
    <section id="articulos">
      <h2>Artículos Destacados</h2>

      <article>
        <header>
          <h3>¿Qué es la Inteligencia Artificial?</h3>
          <p><time datetime="2026-05-01">1 de mayo de 2026</time></p>
        </header>
        <p>
          La IA es la simulación de procesos de inteligencia humana por parte
          de sistemas informáticos, incluyendo aprendizaje, razonamiento y
          autocorrección.
        </p>
      </article>

      <article>
        <header>
          <h3>HTML5 y el Desarrollo Web Moderno</h3>
          <p><time datetime="2026-04-20">20 de abril de 2026</time></p>
        </header>
        <p>
          HTML5 introduce elementos semánticos como <code>&lt;header&gt;</code>,
          <code>&lt;main&gt;</code>, <code>&lt;nav&gt;</code> y
          <code>&lt;footer&gt;</code> que mejoran la accesibilidad y el SEO.
        </p>
      </article>

    </section>

    <!-- Formulario de contacto -->
    <section id="contacto">
      <h2>📬 Contáctanos</h2>
      <form action="#" method="POST">

        <label for="nombre">Nombre:</label>
        <input type="text" id="nombre" name="nombre" placeholder="Tu nombre" required />

        <label for="email">Correo electrónico:</label>
        <input type="email" id="email" name="email" placeholder="tucorreo@email.com" required />

        <label for="mensaje">Mensaje:</label>
        <textarea id="mensaje" name="mensaje" rows="5" placeholder="Escribe tu mensaje..." required></textarea>

        <button type="submit">Enviar mensaje</button>

      </form>
    </section>

  </main>

  <!-- Pie de página -->
  <footer>
    <p>&copy; 2026 Mundo Tech — Todos los derechos reservados</p>
  </footer>

</body>
</html>
```

---

## 🎨 Estilos CSS3 (`style.css`)

```css
/* ===== Reset básico ===== */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* ===== Estilos generales ===== */
body {
  font-family: Arial, sans-serif;
  background-color: #f4f4f4;
  color: #333;
  line-height: 1.6;
}

/* ===== Header ===== */
header {
  background-color: #1a1a2e;
  color: white;
  padding: 1rem 2rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

header h1 {
  font-size: 1.8rem;
}

/* ===== Nav ===== */
nav ul {
  list-style: none;
  display: flex;
  gap: 1.5rem;
}

nav a {
  color: white;
  text-decoration: none;
  font-weight: bold;
  transition: color 0.3s;
}

nav a:hover {
  color: #00aaff;
}

/* ===== Main ===== */
main {
  max-width: 900px;
  margin: 2rem auto;
  padding: 0 1rem;
}

/* ===== Secciones ===== */
section {
  margin-bottom: 2.5rem;
}

section h2 {
  font-size: 1.5rem;
  color: #1a1a2e;
  border-bottom: 2px solid #00aaff;
  padding-bottom: 0.5rem;
  margin-bottom: 1rem;
}

/* ===== Artículos ===== */
article {
  background-color: white;
  border-radius: 8px;
  padding: 1.2rem;
  margin-bottom: 1rem;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.1);
  transition: box-shadow 0.3s;
}

article:hover {
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
}

article h3 {
  color: #1a1a2e;
  margin-bottom: 0.3rem;
}

article time {
  font-size: 0.85rem;
  color: #888;
}

/* ===== Formulario ===== */
form {
  background-color: white;
  padding: 1.5rem;
  border-radius: 8px;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.1);
  display: flex;
  flex-direction: column;
  gap: 0.8rem;
}

label {
  font-weight: bold;
  color: #1a1a2e;
}

input,
textarea {
  padding: 0.6rem;
  border: 1px solid #ccc;
  border-radius: 6px;
  font-size: 1rem;
  transition: border-color 0.3s;
}

input:focus,
textarea:focus {
  border-color: #00aaff;
  outline: none;
}

button[type="submit"] {
  background-color: #00aaff;
  color: white;
  border: none;
  padding: 0.8rem;
  border-radius: 6px;
  font-size: 1rem;
  cursor: pointer;
  transition: background-color 0.3s;
}

button[type="submit"]:hover {
  background-color: #0077cc;
}

/* ===== Footer ===== */
footer {
  background-color: #1a1a2e;
  color: #aaa;
  text-align: center;
  padding: 1rem;
  margin-top: 2rem;
}

/* ===== Responsive ===== */
@media (max-width: 768px) {
  header {
    flex-direction: column;
    text-align: center;
    gap: 0.8rem;
  }

  nav ul {
    flex-direction: column;
    align-items: center;
    gap: 0.5rem;
  }
}
```

---

## ✅ Elementos Semánticos Utilizados

| Etiqueta | Uso en el proyecto |
|----------|--------------------|
| `<header>` | Encabezado con logo y navegación |
| `<nav>` | Menú de navegación principal |
| `<main>` | Contenido principal de la página |
| `<section>` | Agrupación de contenido temático |
| `<article>` | Artículos independientes de tecnología |
| `<footer>` | Pie de página con derechos |
| `<time>` | Fecha de publicación de artículos |
| `<form>` | Formulario de contacto funcional |

---

## 📌 Criterios Aplicados

- [x] Estructura semántica HTML5 completa
- [x] Navegación con `<nav>` y enlaces ancla
- [x] Artículos con `<article>` y `<time>`
- [x] Formulario con validación básica (`required`)
- [x] Estilos con colores, sombras y bordes redondeados
- [x] Efecto `hover` en enlaces, artículos y botón
- [x] Diseño **responsive** con media queries

---

*Actividad desarrollada con HTML5 y CSS3 — Desarrollo Web Básico*
