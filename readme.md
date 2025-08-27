# 🍸 El Refugio Bar - Sitio Web Profesional

Una página web moderna y profesional para un bar, diseñada con las mejores prácticas de desarrollo web y optimizada para conversiones.

## 🌟 Características Principales

### ✨ Diseño y UX
- **Landing page espectacular** con hero section de alto impacto
- **Diseño 100% responsivo** (Mobile First)
- **Animaciones suaves** y efectos visuales atractivos
- **Navegación intuitiva** con scroll suave
- **Paleta de colores profesional** (negro, dorado, grises)

### 🚀 Funcionalidades
- **Botón flotante de WhatsApp** configurable
- **Formulario de contacto** integrado con Formspree
- **Validación en tiempo real** de formularios
- **Efectos de scroll** y animaciones al hacer scroll
- **Menú móvil** completamente funcional
- **Botón "Volver arriba"** para mejor navegación

### 📱 Secciones Incluidas
1. **Hero Section** - Impacto visual inmediato
2. **Servicios** - 6 servicios principales del bar
3. **Sobre Nosotros** - Historia y estadísticas
4. **Testimonios** - Reseñas de clientes
5. **Call to Action** - Conversión optimizada
6. **Contacto** - Formulario y información
7. **Footer** - Enlaces y redes sociales

## 🛠️ Tecnologías Utilizadas

- **HTML5** - Estructura semántica
- **CSS3** - Estilos personalizados y animaciones
- **JavaScript ES6+** - Interactividad y funcionalidad
- **Tailwind CSS** - Framework CSS para diseño rápido
- **Font Awesome** - Iconografía profesional
- **Google Fonts** - Tipografías premium (Playfair Display + Inter)
- **Formspree** - Manejo de formularios

## 📁 Estructura del Proyecto

```
el-refugio-bar/
├── index.html          # Página principal
├── style.css           # Estilos personalizados
├── script.js           # Funcionalidad JavaScript
├── README.md           # Documentación
└── .gitignore          # Archivos a ignorar en Git
```

## 🚀 Instalación y Configuración

### 1. Clonar el Repositorio

```bash
git clone https://github.com/tu-usuario/el-refugio-bar.git
cd el-refugio-bar
```

### 2. Configuración Inicial

#### Configurar Formspree (Formulario de Contacto)
1. Ve a [Formspree.io](https://formspree.io) y crea una cuenta
2. Crea un nuevo formulario
3. Copia el endpoint de tu formulario
4. En `index.html`, línea 442, reemplaza `YOUR_FORM_ID`:
```html
<form id="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

#### Configurar WhatsApp
En `script.js`, línea 318, actualiza el número de teléfono:
```javascript
const phoneNumber = '1234567890'; // Reemplaza con tu número real
```

#### Personalizar Información de Contacto
En `index.html`, actualiza:
- Dirección (líneas 460-462)
- Teléfono (línea 470)
- Email (línea 480)
- Horarios (líneas 490-494)

### 3. Ejecución Local

#### Opción 1: Servidor HTTP Simple (Python)
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

#### Opción 2: Live Server (VS Code)
1. Instala la extensión "Live Server" en VS Code
2. Haz clic derecho en `index.html`
3. Selecciona "Open with Live Server"

#### Opción 3: Servidor Node.js
```bash
npx http-server
```

Visita `http://localhost:8000` en tu navegador.

## 🌐 Despliegue en GitHub Pages

### Paso 1: Subir a GitHub
```bash
git add .
git commit -m "Initial commit: El Refugio Bar website"
git branch -M main
git remote add origin https://github.com/tu-usuario/el-refugio-bar.git
git push -u origin main
```

### Paso 2: Activar GitHub Pages
1. Ve a tu repositorio en GitHub
2. Haz clic en **Settings**
3. Scroll hasta **Pages** en el menú lateral
4. En **Source**, selecciona **Deploy from a branch**
5. Selecciona **main** branch y **/ (root)**
6. Haz clic en **Save**

### Paso 3: Acceder al Sitio
Tu sitio estará disponible en:
```
https://tu-usuario.github.io/el-refugio-bar/
```

⚠️ **Nota**: GitHub Pages puede tardar unos minutos en actualizar.

## ⚙️ Configuraciones Adicionales

### Personalización de Colores
En `style.css`, puedes modificar la paleta de colores:
```css
:root {
  --primary-color: #f59e0b;    /* Dorado */
  --secondary-color: #1f2937;  /* Gris oscuro */
  --accent-color: #ef4444;     /* Rojo para errores */
}
```

### Agregar Google Analytics
En `index.html`, antes del cierre de `</head>`:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_TRACKING_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_TRACKING_ID');
</script>
```

### Configurar Redes Sociales
En `index.html`, actualiza los enlaces de redes sociales (líneas 520-535 y 650-665).

## 📱 Optimizaciones Móviles

- **Diseño Mobile First**: Optimizado primero para móviles
- **Touch Targets**: Botones de mínimo 44px para fácil toque
- **Imágenes Responsivas**: Se adaptan a cualquier pantalla
- **Menú Hamburguesa**: Navegación optimizada para móvil
- **Formularios Táctiles**: Teclados optimizados por tipo de campo

## 🔧 Funcionalidades Técnicas

### Validación de Formularios
- Validación en tiempo real
- Mensajes de error personalizados
- Validación de email y teléfono
- Estados de carga visual

### Efectos de Scroll
- Parallax en hero section
- Animaciones al hacer scroll
- Navegación activa según sección
- Botón "volver arriba"

### Accesibilidad
- Navegación por teclado
- Contraste adecuado
- Textos alternativos
- Focus visible
- Soporte para lectores de pantalla

## 🎨 Personalización de Contenido

### Cambiar Textos
Todos los textos están en español y pueden modificarse directamente en `index.html`:
- Título principal (línea 85)
- Descripción del hero (línea 88)
- Servicios (líneas 110-280)
- Testimonios (líneas 380-440)

### Agregar Nuevos Servicios
Para agregar un nuevo servicio, copia el bloque de código de un servicio existente y modifica:
- Icono (clase Font Awesome)
- Color de fondo (clases Tailwind)
- Título y descripción
- Lista de características

### Modificar Testimonios
Cada testimonio incluye:
- Calificación (estrellas)
- Comentario del cliente
- Nombre y rol del cliente
- Avatar con iniciales

## 🔍 SEO y Performance

### SEO Incluido
- Meta tags optimizados
- Estructura semántica HTML5
- URLs amigables con anclas
- Descripción meta personalizada
- Títulos jerárquicos correctos

### Performance
- CSS y JS minificados en producción
- Imágenes optimizadas
- Lazy loading implementado
- Animaciones optimizadas
- Código JavaScript eficiente

## 🐛 Solución de Problemas

### El formulario no envía emails
1. Verifica que hayas configurado correctamente Formspree
2. Asegúrate de que el endpoint sea correcto
3. Revisa la consola del navegador para errores

### WhatsApp no abre
1. Verifica que el número esté en formato internacional
2. Asegúrate de no incluir espacios o caracteres especiales
3. Prueba el enlace manualmente

### Animaciones no funcionan
1. Verifica que JavaScript esté habilitado
2. Revisa la consola para errores de JavaScript
3. Asegúrate de que todos los archivos estén cargando correctamente

### Problemas de responsive
1. Verifica que el viewport meta tag esté presente
2. Prueba en diferentes dispositivos y navegadores
3. Usa las herramientas de desarrollador para simular dispositivos

## 📞 Soporte

Si necesitas ayuda con la implementación o personalización:

- 📧 Email: soporte@ejemplo.com
- 💬 WhatsApp: +1 (555) 123-4567
- 🐛 Issues: [GitHub Issues](https://github.com/tu-usuario/el-refugio-bar/issues)

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Puedes usarlo libremente para proyectos comerciales y personales.

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Para contribuir:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📈 Roadmap

### Próximas Funcionalidades
- [ ] Sistema de reservas online
- [ ] Galería de fotos
- [ ] Menú digital interactivo
- [ ] Integración con redes sociales
- [ ] Blog/noticias
- [ ] Eventos y calendario
- [ ] Programa de fidelidad
- [ ] PWA (Progressive Web App)

## 🏆 Créditos

- **Diseño**: Inspirado en las mejores prácticas de UX/UI
- **Iconos**: Font Awesome
- **Fuentes**: Google Fonts (Playfair Display, Inter)
- **Framework CSS**: Tailwind CSS
- **Formularios**: Formspree

---

**¡Gracias por elegir El Refugio Bar!** 🍸

*Desarrollado con ❤️ para crear experiencias web excepcionales.*
