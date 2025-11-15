# 🐾 Fundación Patitas Felices - Proyecto HTML/CSS

![Estado](https://img.shields.io/badge/estado-completado-success)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)

## 📋 Descripción del Proyecto

Sitio web estático desarrollado para la **Fundación Patitas Felices**, una organización dedicada al rescate, cuidado y reubicación de animales. El proyecto cumple con todos los requerimientos académicos establecidos.

### Características Principales

- ✅ **100% HTML y CSS Nativo** - Sin dependencias de JavaScript (solo para menú móvil)
- 🎨 **Diseño Responsive** - 3+ breakpoints
- 🎭 **Carrusel CSS Puro** - Automático cada 3 segundos
- 📝 **Formulario con Validación Visual** - Estados error/success simulados con CSS
- ♿ **Accesible** - Semántica HTML5 correcta
- 🐕 **11 Animales en Catálogo** - Cumple requisito mínimo de 8

---

## 🗂️ Estructura del Proyecto

```
proyecto-html-css/
│
├── index.html                    # Página principal
├── README.md                     # Este archivo
│
├── css/
│   ├── index.css                # Estilos página principal
│   ├── style.css                # Estilos globales
│   ├── adopta.css               # Estilos catálogo
│   ├── perfil-animal.css        # Estilos perfil
│   ├── contacto.css             # Estilos formulario
│   └── apoyanos.css             # Estilos apoyanos
│
├── pages/
│   ├── adopta.html              # Catálogo de animales
│   ├── perfil-animal.html       # Detalle de animal
│   ├── contacto.html            # Formulario de contacto
│   └── apoyanos.html            # Donaciones y voluntariado
│
└── img/
    ├── c1.jpg, c2.jpg, c3.jpg   # Imágenes carrusel
    ├── g1.jpg - g4.jpg          # Galería
    └── animales/                # Fotos de animales
        ├── perro1.jpg - perro5.jpg
        ├── gato1.jpg - gato4.jpg
        └── loro1.jpg, loro2.jpg
```

---

## 🚀 Instrucciones de Ejecución

### Opción 1: Apertura Directa
1. Descarga el proyecto
2. Abre `index.html` con tu navegador

### Opción 2: Servidor Local (Recomendado)

**Python 3:**
```bash
python -m http.server 8000
```

**Node.js:**
```bash
npx http-server -p 8000
```

**PHP:**
```bash
php -S localhost:8000
```

Luego visita: `http://localhost:8000`

---

## 📄 Páginas Implementadas

### 🏠 index.html - Página Principal

**Contenido:**
- ✅ Banner hero con nombre, logo y slogan
- ✅ Botón CTA "Adopta"
- ✅ Carrusel CSS automático (3 slides, 12s loop)
- ✅ 4 secciones destacadas (Adopta, Donaciones, Voluntariado, Contacto)
- ✅ Misión y Visión lado a lado
- ✅ 3 testimonios de adoptantes
- ✅ Galería de 8 imágenes
- ✅ Footer con flexbox

**Tecnologías:**
- CSS Grid para secciones
- Flexbox para header/footer
- `@keyframes` para carrusel
- Variables CSS

---

### 🐕 pages/adopta.html - Catálogo de Animales

**Contenido:**
- ✅ Grid responsive con 11 animales
- ✅ Información: nombre, edad, tamaño, raza
- ✅ Estados: "Disponible" y "Adoptado"
- ✅ Botón "Ver perfil" en cada tarjeta
- ✅ Variedad: 5 perros, 4 gatos, 2 loros

**Características:**
- Grid auto-responsive con `minmax(280px, 1fr)`
- Badges con colores diferenciados
- Hover effects en tarjetas
- Imágenes de 250px altura

---

### 📋 pages/perfil-animal.html - Detalle de Animal

**Contenido:**
- ✅ Imagen grande del animal
- ✅ Información detallada (raza, edad, tamaño, sexo, peso, color)
- ✅ Historia del rescate
- ✅ Lista de personalidad
- ✅ Estado de salud (vacunas, esterilización, desparasitación, microchip)
- ✅ Hogar ideal recomendado
- ✅ 4 animales relacionados en carrusel horizontal
- ✅ CTA "Solicitar adopción"

**Layout:**
- Grid 2 columnas en desktop
- Grid info 2x3
- Cards relacionados responsivas

---

### 📧 pages/contacto.html - Formulario de Contacto

**Contenido:**
- ✅ **Campos obligatorios marcados con (\*)**:
  - Nombre
  - Apellidos
  - Ciudad
  - Teléfono
  - Email
  - Tipo de consulta (select)
  - Mensaje (textarea)
  - Checkbox de términos
- ✅ **Validación visual con CSS**:
  - Estados `.error` y `.success`
  - Mensajes de error mostrados/ocultados
  - Ejemplos visuales incluidos
- ✅ **Información de contacto**:
  - Email, teléfono, dirección
  - Horarios de atención
  - Links a redes sociales
- ✅ **4 Preguntas frecuentes**

**Layout:**
- Grid 2:1 (formulario:sidebar)
- Sidebar con 3 cards
- FAQ en grid responsive

---

### 💝 pages/apoyanos.html - Donaciones y Voluntariado

**Contenido:**
- ✅ Sección de donaciones
- ✅ Sección de voluntariado
- ✅ Requisitos y beneficios
- ✅ Formas de apoyo
- ✅ CTA a formulario de contacto

---

## 🎨 Paleta de Colores

```css
--bg: #F4F7F6           /* Fondo general */
--surface: #FFFFFF      /* Tarjetas */
--primary: #2BA68B      /* Verde principal */
--primary-dark: #207F68 /* Verde oscuro */
--accent: #FFD766       /* Amarillo acento */
--text: #222            /* Texto principal */
--muted: #6B6B6B        /* Texto secundario */
--success: #2ECC71      /* Verde éxito */
--error: #E74C3C        /* Rojo error */
```

---

## 📱 Breakpoints Responsive (3+)

| Dispositivo | Ancho | Características |
|------------|-------|-----------------|
| **Desktop** | >1024px | Layout completo, grids de 4 columnas |
| **Tablet** | 768px - 1024px | Grids de 2 columnas, navegación adaptada |
| **Móvil** | 480px - 768px | Grids de 1 columna, menú hamburguesa |
| **Móvil Pequeño** | <480px | Fuentes reducidas, padding ajustado |

---

## ✨ Componentes Interactivos (CSS Puro)

### 1. Carrusel Automático
```css
@keyframes slide {
    0% { transform: translateX(0); }
    33% { transform: translateX(-100%); }
    66% { transform: translateX(-200%); }
    100% { transform: translateX(0); }
}
```
- 3 slides
- Cambio cada 3 segundos (12s total)
- Loop infinito

### 2. Validación de Formulario
```css
.form-group.error input { border-color: var(--error); }
.form-group.success input { border-color: var(--success); }
```
- Estados simulados con clases CSS
- Mensajes mostrados con `display: block`
- Ejemplo visual incluido

### 3. Menú Responsive
- Checkbox hack para toggle
- Transiciones suaves
- Hamburguesa animada

---

## ✅ Checklist de Requerimientos

### Página de Inicio
- [x] Banner principal con nombre, logo, slogan
- [x] Botón CTA "Conócenos/Adopta"
- [x] Carrusel CSS automático (3 segundos)
- [x] Secciones destacadas (4 links internos)
- [x] Testimonios (3 citas)
- [x] Visión y Misión lateralmente
- [x] Galería de imágenes

### Catálogo de Animales
- [x] Mínimo 8 animales (11 implementados)
- [x] Grid de tarjetas
- [x] Información: imagen, nombre, edad, tamaño/raza
- [x] Estados: "Disponible" / "Adoptado"
- [x] Botón "Ver perfil"

### Perfil de Animal
- [x] Foto grande
- [x] Descripción completa (historia, salud, comportamiento)
- [x] Características (edad, sexo, tamaño, etc.)
- [x] CTA "Solicitar adopción"
- [x] Sección de animales relacionados

### Formulario de Contacto
- [x] Campos obligatorios marcados (\*)
- [x] Nombre, Apellidos, Ciudad, Email, Teléfono
- [x] Select tipo de consulta
- [x] Textarea mensaje
- [x] Validación visual con CSS
- [x] Estados error/success
- [x] Información de contacto directo
- [x] Links a redes sociales

### Footer
- [x] Nombre de la fundación
- [x] Año + Copyright
- [x] Correo de contacto
- [x] Enlace al desarrollador
- [x] Implementado con Flexbox

### General
- [x] Código organizado en carpetas (HTML/CSS separados)
- [x] Responsive con 3+ breakpoints
- [x] Componentes interactivos simulados (carrusel, validación)
- [x] README.md con documentación
- [x] Sin JavaScript excepto menú móvil

---

## 🎯 Características Destacadas

### Carrusel CSS Puro
- No requiere JavaScript
- Animación fluida con `@keyframes`
- 3 slides con timing preciso
- Caption overlay con gradiente

### Grid Responsivo Inteligente
```css
grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
```
- Se adapta automáticamente al espacio
- Sin media queries específicos
- Mantiene proporciones

### Validación Visual Avanzada
- Clases `.error` y `.success`
- Pseudoclases `:focus`, `:valid`
- Mensajes contextuales
- Ejemplo en vivo para demostración

---

## 📸 Capturas de Pantalla

### Desktop
- Página principal con hero y carrusel
- Catálogo de animales en grid 3x4
- Perfil de animal layout 2 columnas
- Formulario con sidebar

### Móvil
- Diseño apilado vertical
- Menú hamburguesa funcional
- Cards de ancho completo
- Formulario de una columna

---

## 🔧 Tecnologías Utilizadas

- **HTML5**: Semántica correcta (`<section>`, `<nav>`, `<article>`)
- **CSS3**:
  - CSS Grid
  - Flexbox
  - Variables (Custom Properties)
  - Media Queries
  - Keyframe Animations
  - Pseudo-classes y Pseudo-elements
  - Transitions

---

## 📝 Notas del Desarrollador

### Decisiones de Diseño

1. **Paleta Verde/Amarillo**: Transmite naturaleza, esperanza y alegría
2. **Grid Auto-responsive**: Reduce código y mejora mantenibilidad
3. **Carrusel CSS**: Evita dependencias JavaScript innecesarias
4. **Sidebar en Contacto**: Maximiza conversión con información accesible

### Mejoras Futuras Sugeridas

- [ ] Backend para formulario de contacto
- [ ] Base de datos para animales
- [ ] Sistema de búsqueda y filtros
- [ ] Panel de administración
- [ ] Integración con redes sociales
- [ ] Sistema de citas en línea
- [ ] Pasarela de pagos para donaciones

---

## 🎓 Información Académica

**Proyecto**: Maqueta Web Estática  
**Institución**: [Tu Institución]  
**Materia**: Diseño Web / HTML y CSS  
**Fecha**: Noviembre 2025  
**Desarrollador**: Joel Martínez

---

## 📞 Contacto de la Fundación

- **Email**: contacto@patitasfelices.org
- **Teléfono**: +57 323 877 0327
- **Ubicación**: Piedecuesta, Santander, Colombia

### Redes Sociales
- Facebook: @PatitasFelices
- Instagram: @patitas_felices
- Twitter: @PatitasFelices

---

## 📄 Licencia

Este proyecto es de código abierto con fines educativos.

---

## 🙏 Agradecimientos

- A la Fundación Patitas Felices por su noble labor
- A los docentes por su guía en el proyecto
- A todos los que apoyan la causa animal

---

**¡Ayúdanos a darles una segunda oportunidad! 🐾**

---

## ⚠️ Importante

**ANTES DE IMPLEMENTAR CÓDIGO**: Los wireframes deben ser aprobados por el docente según los requerimientos del proyecto.