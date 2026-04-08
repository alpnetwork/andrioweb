# ANDRION AI CONSULTING — WEB PREMIUM

Web completamente nueva y premium para Andrion AI Consulting, lista para subir a WordPress.

## 📁 Estructura de archivos

```
andrion-web/
├── index.html              → Página de Inicio
├── sobre-nosotros.html     → Sobre Nosotros (CEO, equipo, valores)
├── pricing.html            → Precios y servicios
├── trabajos.html           → Portfolio de proyectos
├── contacto.html           → Formulario e info de contacto
├── css/
│   └── style.css           → TODOS los estilos (editar colores aquí)
├── js/
│   └── script.js           → Animaciones y formulario
├── images/                 → Carpeta para tus imágenes
└── README.md               → Este archivo
```

## 🎨 Cómo cambiar los colores

Abre `css/style.css` y en las primeras líneas verás `:root`. Ahí puedes cambiar:

```css
--brand: #ff914d;          /* Color principal de marca */
--brand-dark: #e67332;     /* Versión oscura */
--brand-light: #ffb27a;    /* Versión clara */
```

Cambias esos valores y TODA la web se actualiza automáticamente.

## ✏️ Cómo editar contenido

Todos los archivos HTML tienen comentarios claros en español marcando las zonas editables:

```html
<!-- ============ EDITA AQUÍ EL TÍTULO PRINCIPAL ============ -->
<h1>Tu nuevo título aquí</h1>
```

Busca los comentarios `EDITA AQUÍ` y modifica el texto entre las etiquetas.

## 🚀 Cómo subirlo a WordPress

Tienes 3 opciones según tu nivel técnico:

### Opción 1 — Plugin "HTML Pages With Shortcodes" (MÁS FÁCIL)

1. Instala el plugin **HTML Pages With Shortcodes** desde WordPress
2. Crea una nueva "HTML Page" para cada archivo HTML
3. Pega el contenido de cada archivo
4. Sube las carpetas `css/`, `js/` e `images/` vía FTP a `/wp-content/uploads/andrion/`
5. Ajusta las rutas en el HTML (`css/style.css` → `/wp-content/uploads/andrion/css/style.css`)

### Opción 2 — Subida por FTP (RECOMENDADA)

1. Conecta a tu hosting con FileZilla o similar
2. Navega a la carpeta pública de tu dominio (`public_html/` o `htdocs/`)
3. Crea una subcarpeta (ej: `nueva-web/`)
4. Sube TODA la estructura de `andrion-web/` allí
5. Accede desde `tudominio.com/nueva-web/`
6. Cuando te guste, mueve los archivos a la raíz reemplazando los antiguos

### Opción 3 — Convertir en tema WordPress completo

Si quieres que sea un tema nativo de WordPress, necesitarás:
- Renombrar `index.html` → `index.php`
- Crear `style.css` con cabecera de tema
- Crear `functions.php`
- Adaptar las rutas con `<?php bloginfo('template_url'); ?>`

Esta opción requiere conocimientos de desarrollo. Contacta con un desarrollador si no estás seguro.

## 📝 Formulario de contacto en WordPress

El formulario actual usa JavaScript simulado. Para hacerlo funcional en WordPress:

1. Instala el plugin **Contact Form 7** (gratis)
2. Crea un nuevo formulario con los mismos campos
3. Abre `contacto.html` y busca el comentario:
   ```
   NOTA PARA WORDPRESS
   ```
4. Reemplaza el `<form>` entero por el shortcode:
   ```
   [contact-form-7 id="TU_ID" title="Contacto"]
   ```

## 🖼️ Añadir imágenes

1. Guarda tus imágenes en la carpeta `images/`
2. En cualquier HTML, usa:
   ```html
   <img src="images/nombre-archivo.jpg" alt="Descripción">
   ```

### Para la foto del CEO

Abre `sobre-nosotros.html` y busca el comentario `PARA PONER LA FOTO DEL CEO`. Reemplaza la letra "A" por:

```html
<img src="images/ceo.jpg" alt="Andrei P. Lupu" style="width:100%;height:100%;object-fit:cover;">
```

## 🎯 Páginas incluidas

| Página | Descripción |
|--------|-------------|
| **index.html** | Hero con mockup de chat, stats, bento grid de servicios, integraciones, 3 pilares |
| **sobre-nosotros.html** | Historia, CEO con cita, equipo, 6 garantías, 4 valores |
| **pricing.html** | Proceso en 4 pasos, 3 planes (Starter €497, Business €1.497, Enterprise €3.997+), detalle de 4 servicios |
| **trabajos.html** | 9 proyectos de ejemplo con iconos, tags, resultados medibles |
| **contacto.html** | Info de contacto (teléfonos, email, WhatsApp, Calendly), horarios, formulario |

## 📞 Datos de contacto actuales (en todas las páginas)

- **Atención al cliente:** +34 655 73 76 90
- **Servicio técnico:** +34 654 25 51 88
- **Email:** info@andrion.es
- **WhatsApp:** https://wa.link/kukgzl
- **Presupuesto:** https://wa.link/f5chp9
- **Calendly:** https://calendly.com/apl-network/30min
- **Horarios:** Lun-Vie 10:00-20:00 · Sáb-Dom 10:00-14:00

Si quieres cambiar estos datos, búscalos con Ctrl+F en cada HTML y reemplázalos.

## 💡 Tips

- **Tipografía:** La web usa Inter desde Google Fonts (se carga automáticamente)
- **Iconos:** Todos los iconos son SVG inline de Lucide Icons (no necesitas librerías externas)
- **Responsive:** La web funciona perfectamente en móvil, tablet y escritorio
- **Animaciones:** Los elementos con clase `fade-in` aparecen al hacer scroll

---

Cualquier duda, revisa los comentarios dentro de cada archivo HTML y CSS. Todo está marcado en español.
