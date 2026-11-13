# 🚲 Rueda Libre & Campaña Rueda Nocturna

> Ecosistema web corporativo y landing page para el alquiler de bicicletas y rutas nocturnas guiadas en Medellín, Colombia.

[![W3C HTML5 Valid](https://img.shields.io/badge/W3C-HTML5%20Valid-brightgreen)](https://validator.w3.org/)
[![Tailwind CSS v4](https://img.shields.io/badge/Tailwind%20CSS-v4.3.5-38bdf8)](https://tailwindcss.com/)
[![Bootstrap 5.3](https://img.shields.io/badge/Bootstrap-v5.3.3-7952b3)](https://getbootstrap.com/)
[![WCAG 2.1 AA](https://img.shields.io/badge/WCAG%202.1-Nivel%20AA%2FAAA-emerald)](https://www.w3.org/WAI/WCAG21/quickref/)
[![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-blue)](https://juan98698.github.io/rueda-libre/)

---

## 🌐 Enlaces Públicos en Línea (GitHub Pages)

* **Sitio Web Principal (v2.0)**: [https://juan98698.github.io/rueda-libre/](https://juan98698.github.io/rueda-libre/)
* **Landing Page Campaña Rueda Nocturna**: [https://juan98698.github.io/rueda-libre/nocturna/](https://juan98698.github.io/rueda-libre/nocturna/)
* **Kit de Componentes y Design System**: [https://juan98698.github.io/rueda-libre/nocturna/componentes.html](https://juan98698.github.io/rueda-libre/nocturna/componentes.html)
* **Repositorio en GitHub**: [https://github.com/Juan98698/rueda-libre](https://github.com/Juan98698/rueda-libre)

---

## 📖 Descripción del Proyecto

**Rueda Libre** es una empresa de movilidad sostenible y turismo urbano en Medellín dedicada al alquiler de bicicletas para todos los gustos y terrenos. A dos días del lanzamiento de su nueva iniciativa turística, se desarrolló y acopló la campaña **"Rueda Nocturna"**, un producto digital optimizado bajo el enfoque *mobile-first*, adaptado para tráfico proveniente de redes sociales (Instagram, TikTok), con soporte nativo para **modo oscuro**, validación accesible de inscripciones y navegación bidireccional continua con el sitio institucional.

---

## 🗺️ Mapa del Sitio y Páginas

```
rueda-libre/
├── index.html                  # Inicio del sitio institucional con carrusel interactivo v2.0
├── paginas/
│   ├── tarifas.html            # Tarifas de alquiler y tabla de rutas diurnas
│   └── reservas.html           # Formulario institucional de reserva de flota
├── nocturna/
│   ├── index.html              # Landing page oficial de la campaña Rueda Nocturna
│   ├── componentes.html        # Librería y kit de componentes del Design System
│   └── src/
│       ├── input.css           # Entrada con directivas @theme y @layer components
│       └── output.css          # CSS compilado y minificado por Tailwind CLI (42.3 KB)
├── css/
│   └── styles.css              # Hoja de estilos principal con variables corporativas
├── img/                        # Recursos gráficos y fotografías optimizadas en proporción 3:2
└── bitacora.txt                # Registro detallado de pruebas, contrastes y tiempos reales
```

---

## 🛠️ Tecnologías y Estándares Aplicados

* **HTML5 Semántico**: Uso riguroso de `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<figure>`, `<footer>`, `<fieldset>`, `<legend>` y `<address>`. **Validado con 0 errores en el W3C Validator**.
* **CSS3 Modular**: Modelo de caja universal (`box-sizing: border-box`), arquitectura de tokens en `:root` y diseño responsivo sin desbordamiento.
* **Bootstrap 5.3.3**: Barra de navegación global y carrusel rectangular interactivo ($3:2$) con 4 diapositivas en el home.
* **Tailwind CSS v4 (CLI)**: Compilación utility-first de alto rendimiento con `@theme`, personalización de 6 colores institucionales y variantes accesibles `dark:`.
* **Abstracción Limpia (`@apply`)**: Consolidación de 3 variantes de botones (`.btn-primary`, `.btn-secondary`, `.btn-outline`) en `@layer components`, eliminando redundancia en el marcado.
* **Tipografías Web Google Fonts**: *Montserrat* (títulos de alto impacto) y *Open Sans* (cuerpo y lectura prolongada).
* **Accesibilidad Web (WCAG 2.1 AA/AAA)**: 
  * 100% operable solo con teclado con anillo de foco visible (`focus:ring-2 focus:ring-offset-2`).
  * Validación nativa estricta (`required`, `minlength`, `pattern="3[0-9]{9}"`, `min`, `max`).
  * Contrastes certificados superiores a 4.5:1 en modo claro y hasta 11.08:1 en modo oscuro.

---

## 🎨 Paleta de Color Institucional y Tokens

| Nombre de Color | Código Hex | Variable CSS / Bootstrap | Utility Tailwind (`@theme`) | Ratio de Contraste |
| :--- | :--- | :--- | :--- | :--- |
| **Crema** | `#FAF6EF` | `--color-crema` / `--bs-light` | `bg-crema` / `text-crema` | Fondo base cálido |
| **Azul Noche** | `#14213D` | `--color-azul-noche` / `--bs-dark` | `bg-azul-noche` / `text-azul-noche` | **14.83:1** sobre crema (AAA) |
| **Verde Ruta** | `#1E7A4F` | `--color-verde` / `--bs-primary` | `bg-verde-ruta` / `text-verde-ruta` | **5.31:1** en claro (AA) |
| **Amarillo Farol** | `#FFD166` | `--color-amarillo-farol` / `--bs-warning` | `bg-amarillo-farol` / `text-amarillo-farol` | **11.08:1** en oscuro (AAA) |
| **Naranja Pedal** | `#F39A2B` | `--color-naranja` / `--bs-danger` | `bg-naranja-pedal` | 3.12:1 (Bordes y acentos) |
| **Gris Asfalto** | `#5B6470` | `--color-gris` / `--bs-secondary` | `bg-gris-asfalto` / `text-gris-asfalto` | 4.88:1 en textos secundarios |

> **Nota de Accesibilidad:** Para resolver el problema de bajo contraste de Verde Ruta sobre Azul Noche (3.01:1), se implementó **Amarillo Farol (`#FFD166`)** como color de acento nocturno en modo oscuro, alcanzando un contraste sobresaliente de **11.08:1 (Nivel AAA)**.

---

## 📊 Veredicto Técnico: Bootstrap vs Tailwind CSS

Como parte del MiniReto 8, se midieron los recursos reales en red y se redactó una comparativa justificada con datos de ambas versiones:

### Medición Real de Recursos (Network DevTools)

| Recurso / Framework | Tamaño en Disco | Transferencia (Gzip) | Dependencia JS | Tiempo de Carga (4G) |
| :--- | :--- | :--- | :--- | :--- |
| **Tailwind CSS v4 (CLI --minify)** | **42.3 KB** | **6.5 KB** | **0 KB (Sin JS)** | **~45 ms** |
| Bootstrap 5.3 CSS (`bootstrap.min.css`) | 232.0 KB | 34.2 KB | - | ~210 ms |
| Bootstrap 5.3 JS (`bootstrap.bundle.min.js`) | 80.0 KB | 23.5 KB | 80.0 KB (Obligatorio) | ~180 ms |
| **Total Stack Bootstrap v2.0** | **312.0 KB** | **57.7 KB** | **80.0 KB** | **~390 ms** |

* **Conclusión:** El bundle final de Tailwind CSS es un **86.4% más liviano en transferencia de red** y no bloquea el hilo principal con runtime de JavaScript.

### Análisis en Cuatro Criterios

1. **Curva de Aprendizaje:** Bootstrap es más rápido en el primer día porque provee componentes prediseñados (`.btn`, `.navbar`), pero se vuelve complejo cuando el cliente exige salir de su cuadrícula estándar. Tailwind requiere conocer CSS a fondo, pero una vez dominadas sus utilidades, la velocidad de desarrollo es insuperable.
2. **Personalización y Marca:** Bootstrap impone una identidad genérica y modificar sus temas requiere compilar Sass o sobreescribir especificidad. Tailwind se adapta al 100% al diseño corporativo mediante `@theme` directamente en CSS.
3. **Tamaño Final:** Bootstrap descarga componentes que jamás se usan (modales, acordeones, paginadores). Tailwind realiza *purge* automático y solo incluye las clases utilizadas en el HTML.
4. **Casos de Uso:** Bootstrap es ideal para tableros administrativos (dashboards) o prototipos rápidos internos. Tailwind CSS es la elección profesional para sitios comerciales, landings de conversión y marcas con identidad única.

**Recomendación Final para Rueda Libre:** Se recomienda migrar el sitio institucional completo a **Tailwind CSS**, conservando la estructura de componentes creada con `@apply` para maximizar la velocidad en conexiones móviles y unificar todo el código en un único flujo de trabajo.

---

## ⏱️ Registro de Pruebas Contrarreloj (Bitácora)

Todas las pruebas en tiempo límite fueron superadas con holgura:

| Reto / Sesión | Objetivo Técnico | Tiempo Límite | Tiempo Real | Estado |
| :--- | :--- | :--- | :--- | :--- |
| **Contrarreloj 1** | Formulario accesible con 9 campos, 3 fieldsets y validación nativa | 40 min | **22 min** | Superado (18 min a favor) |
| **Contrarreloj 2** | Integración del ecosistema, rutas relativas y carrusel 3:2 | 40 min | **16 min** | Superado (24 min a favor) |
| **Contrarreloj 3** | Sección de Planes con Grid, Flexbox y card "Más elegido" destacada | 45 min | **17 min** | Superado (28 min a favor) |

---

## 📸 Capturas de Pantalla del Ecosistema

### 1. Vista de Escritorio (Landing Rueda Nocturna a 1280 px)
La cuadrícula organiza las rutas en 3 columnas y la sección de planes en 3 tarjetas de igual altura con botones perfectamente alineados.

### 2. Vista de Celular (Mobile First a 360 px)
Todo el contenido fluye verticalmente en una columna fluida sin scroll horizontal ni desbordamientos táctiles.

### 3. Modo Oscuro Accesible (`prefers-color-scheme: dark`)
Fondo en Azul Noche (`#14213D`), tarjetas translúcidas con backdrop blur y acentos en Amarillo Farol (`#FFD166`) con contraste WCAG AAA.

---

## 🎤 Guion de la Demo (3 Minutos)

Para presentar el proyecto ante el director de Nodo Digital y el cliente:

* **0:00 - 0:45 | Contexto y Sitio Principal:**
  *"Buenas tardes. Rueda Libre necesitaba expandir su negocio hacia el turismo nocturno en Medellín. Aquí vemos el sitio institucional v2.0 con un carrusel rectangular interactivo cuya cuarta diapositiva invita a vivir la experiencia de Rueda Nocturna. Al hacer clic, viajamos sin fricción a la nueva landing de campaña."*
* **0:45 - 1:45 | Recorrido de la Landing y Conversión:**
  *"La landing recibe al usuario con una propuesta de valor clara, la ficha técnica de las 3 rutas guiadas, el proceso en 4 pasos y la nueva sección de Planes, donde destacamos el Plan Pareja como el 'Más elegido'. Al final, el usuario se inscribe en un formulario semántico 100% validado que no permite envíos con datos incompletos ni errores de digitación."*
* **1:45 - 2:30 | Mobile-First y Modo Oscuro:**
  *"Como el 85% del tráfico llega de redes sociales, activamos la vista de celular a 360 px: no hay scroll horizontal, el menú se sintetiza y los botones son táctiles. Además, si el sistema del ciclista está en modo oscuro, la interfaz cambia fluidamente a Azul Noche y Amarillo Farol con contraste AAA certificado."*
* **2:30 - 3:00 | Decisiones Técnicas y Cierre:**
  *"Tomamos dos decisiones clave: primero, unificar la marca con tokens `@theme` en Tailwind v4 para garantizar accesibilidad automática. Segundo, lograr un bundle de solo 42 KB que carga 86% más rápido que Bootstrap en redes 4G. El ecosistema está publicado en GitHub Pages y listo para recibir inscripciones hoy mismo."*

---

## 👨‍💻 Autor y Créditos

* **Desarrollador:** Juan Manuel Cardona
* **Proyecto:** Rueda Libre & Rueda Nocturna
* **Programa:** Cohorte 8 — Desarrollo Web Frontend
* **Institución:** Riwi / Nodo Digital / Ruta N — Medellín, Colombia (2026)

