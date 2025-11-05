# Newsletter Academia Lanzarote - Cursos Gratuitos

Plantilla de newsletter profesional para promocionar cursos gratuitos dirigidos a trabajadores y desempleados residentes en Lanzarote.

## 📋 Contenido

Esta newsletter incluye:

### Cursos Prioritarios para Ocupados (4 cursos):
1. **MF1208_1** - Operaciones Auxiliares de Mantenimiento de Sistemas Microinformáticos
2. **MF1207_1** - Operaciones Auxiliares de Montaje de Componentes Informáticos
3. **MF1019_2** - Apoyo Psicosocial, Atención Relacional y Comunicativa en Instituciones
4. **MF0836_2** - Montaje de Instalaciones Solares Fotovoltaicas

### Cursos Prioritarios para Desempleados (2 cursos):
5. **MF0256_1** - Elaboración Culinaria Básica
6. **MF0250_2** - Atención y Apoyo Psicosocial Domiciliario

## 🚀 Cómo Usar Esta Plantilla

### Paso 1: Preparar las Imágenes

1. Descarga o crea **8 imágenes** (1 cabecera + 1 logo footer + 6 cursos)
2. Consulta el archivo `images/README.md` para ver las especificaciones y sugerencias de cada imagen
3. Formato recomendado cursos: **600x200 píxeles, JPG, máximo 100KB**
4. Coloca las imágenes en la carpeta `images/` con estos nombres:
   - **`header-logo.jpg`** (OBLIGATORIA - Logo/banner de cabecera 600x200px)
   - **`logo-footer.png`** (OBLIGATORIA - Logo pequeño del centro 120px ancho)
   - `curso-mantenimiento-sistemas.jpg`
   - `curso-montaje-componentes.jpg`
   - `curso-apoyo-psicosocial.jpg`
   - `curso-solar-fotovoltaica.jpg`
   - `curso-elaboracion-culinaria.jpg`
   - `curso-atencion-domiciliaria.jpg`

### Paso 2: Personalizar los Enlaces de Formulario

Abre el archivo `newsletter-template.html` y busca estas secciones para reemplazar las URLs:

```html
<!-- Busca y reemplaza estas 6 URLs -->
URL_FORMULARIO_CURSO_1  → Enlace al formulario del MF1208_1
URL_FORMULARIO_CURSO_2  → Enlace al formulario del MF1207_1
URL_FORMULARIO_CURSO_3  → Enlace al formulario del MF1019_2
URL_FORMULARIO_CURSO_4  → Enlace al formulario del MF0836_2
URL_FORMULARIO_CURSO_5  → Enlace al formulario del MF0256_1
URL_FORMULARIO_CURSO_6  → Enlace al formulario del MF0250_2
```

**Ejemplo:**
```html
<!-- Antes -->
<a href="URL_FORMULARIO_CURSO_1" style="...">

<!-- Después -->
<a href="https://tudominio.com/formulario-mf1208" style="...">
```

### Paso 3: Personalizar Información de Contacto

En el **footer** de la newsletter, actualiza:

```html
<!-- Busca esta sección al final del HTML -->
📧 info@academialanzarote.com | 📞 928 XXX XXX
```

Reemplázalo con tus datos reales:
```html
📧 tumail@tudominio.com | 📞 928 123 456
```

### Paso 4: Enviar la Newsletter

#### Opción A: Usando un Servicio de Email Marketing (Recomendado)

1. **MailChimp**, **SendGrid**, **Mailjet** o similar
2. Crea una nueva campaña
3. Selecciona "Código HTML personalizado"
4. Copia y pega el contenido completo de `newsletter-template.html`
5. Sube las imágenes a tu servidor o usa las URLs de las imágenes alojadas
6. Realiza una prueba enviándote un email de test
7. Envía a tu lista de contactos

#### Opción B: Usando un Cliente de Correo

1. Abre el archivo HTML en un navegador
2. Selecciona todo (Ctrl+A / Cmd+A)
3. Copia el contenido renderizado
4. Pega en un nuevo correo de Gmail/Outlook
5. Verifica que las imágenes se vean correctamente

**⚠️ Nota sobre las imágenes:** Para que las imágenes se vean en los emails de tus destinatarios, debes:
- Subirlas a un servidor web (tu sitio web, servicio de hosting de imágenes, etc.)
- Reemplazar las rutas locales por URLs completas:

```html
<!-- Antes -->
<img src="images/curso-mantenimiento-sistemas.jpg" alt="...">

<!-- Después -->
<img src="https://tudominio.com/newsletter/images/curso-mantenimiento-sistemas.jpg" alt="...">
```

## ✨ Características

- ✅ **Responsive Design**: Se adapta perfectamente a móviles y tablets
- ✅ **Compatible con Clientes de Email**: Diseñado con tablas para máxima compatibilidad
- ✅ **Estilos Inline**: Todos los estilos están inline para evitar problemas con clientes de correo
- ✅ **Diseño Profesional**: Colores modernos con gradientes atractivos
- ✅ **Call-to-Action Claros**: Botones destacados para cada curso
- ✅ **Secciones Diferenciadas**: Distinción visual entre cursos para ocupados y desempleados
- ✅ **Fácil de Personalizar**: Estructura clara y comentarios en el código

## 🎨 Personalización Avanzada

### Esquema de Colores

La newsletter utiliza una paleta de **amarillo/dorado (#eab003)** y **negro (#333333)**:

**Botones de CTA (Todos los cursos):**
```css
background-color: #eab003;  /* Amarillo/Dorado */
color: #000000;  /* Texto negro para contraste */
```

**Sección Cursos para Ocupados:**
```css
border-top: 3px solid #eab003;  /* Borde amarillo */
color: #eab003;  /* Título amarillo */
```

**Sección Cursos para Desempleados:**
```css
border-top: 3px solid #333333;  /* Borde negro */
color: #333333;  /* Título negro */
```

Para cambiar estos colores, busca y reemplaza los códigos hexadecimales en el archivo HTML.

### Modificar Descripciones

Las descripciones de los cursos están en párrafos `<p>` dentro de cada tarjeta de curso. Puedes editarlas directamente en el HTML.

### Añadir o Quitar Cursos

Cada curso está contenido en un bloque `<tr><td>...</td></tr>`. Puedes duplicar estas secciones para añadir más cursos o eliminarlas para reducir el número.

## 📱 Vista Previa

Para ver cómo se verá la newsletter:

1. Abre `newsletter-template.html` en tu navegador web
2. Redimensiona la ventana para simular diferentes tamaños de pantalla
3. Verifica que todos los enlaces funcionen correctamente

## 🔧 Requisitos Técnicos

- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Editor de texto o código (VS Code, Sublime Text, Notepad++, etc.)
- Servicio de email marketing o cliente de correo
- Servidor web para alojar las imágenes (opcional pero recomendado)

## 📞 Soporte

Si necesitas ayuda para personalizar o enviar esta newsletter, consulta:
- Documentación de tu servicio de email marketing
- Guías de HTML para emails: [litmus.com](https://litmus.com)
- Herramienta de test: [mail-tester.com](https://www.mail-tester.com)

## 📄 Licencia

Esta plantilla es de libre uso para Academia Lanzarote y sus fines educativos.

---

**¡Buena suerte con tus campañas de newsletter! 🚀**
