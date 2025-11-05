# Guía Rápida de Personalización

Este documento te ayudará a personalizar rápidamente la newsletter para tu academia.

## ✏️ Checklist de Personalización

Antes de enviar tu newsletter, asegúrate de completar estos pasos:

### ☐ 1. Enlaces de Formularios (OBLIGATORIO)

Busca en `newsletter-template.html` estos textos y reemplázalos con las URLs reales:

```
URL_FORMULARIO_CURSO_1  →  https://...
URL_FORMULARIO_CURSO_2  →  https://...
URL_FORMULARIO_CURSO_3  →  https://...
URL_FORMULARIO_CURSO_4  →  https://...
URL_FORMULARIO_CURSO_5  →  https://...
URL_FORMULARIO_CURSO_6  →  https://...
```

**Cómo hacerlo:**
1. Abre `newsletter-template.html` en tu editor de texto
2. Usa Ctrl+F (Cmd+F en Mac) para buscar "URL_FORMULARIO_CURSO_1"
3. Reemplaza por la URL real de tu formulario
4. Repite para los 6 cursos

### ☐ 2. Imágenes (OBLIGATORIO)

Agrega 6 imágenes a la carpeta `images/`:
- ✓ curso-mantenimiento-sistemas.jpg
- ✓ curso-montaje-componentes.jpg
- ✓ curso-apoyo-psicosocial.jpg
- ✓ curso-solar-fotovoltaica.jpg
- ✓ curso-elaboracion-culinaria.jpg
- ✓ curso-atencion-domiciliaria.jpg

**Si vas a enviar por email marketing:** Necesitas URLs completas de las imágenes.

Busca todas las etiquetas `<img src="images/...">` y reemplázalas por URLs completas:

```html
<!-- Antes -->
<img src="images/curso-mantenimiento-sistemas.jpg" alt="...">

<!-- Después -->
<img src="https://tudominio.com/img/curso-mantenimiento-sistemas.jpg" alt="...">
```

Hay **6 imágenes** que cambiar. Busca en el archivo:
```
images/curso-mantenimiento-sistemas.jpg
images/curso-montaje-componentes.jpg
images/curso-apoyo-psicosocial.jpg
images/curso-solar-fotovoltaica.jpg
images/curso-elaboracion-culinaria.jpg
images/curso-atencion-domiciliaria.jpg
```

### ☐ 3. Información de Contacto (RECOMENDADO)

En el footer, busca:
```html
📧 info@academialanzarote.com | 📞 928 XXX XXX
```

Reemplaza con:
```html
📧 tucorreo@tudominio.com | 📞 928 123 456
```

### ☐ 4. Nombre de la Academia (OPCIONAL)

Si tu academia tiene un nombre diferente, busca:
```
Academia Lanzarote
```

Y reemplázalo por el nombre que prefieras (aparece 3 veces en el documento).

## 🎯 Ejemplo de URLs de Formularios

Aquí tienes ejemplos de cómo podrían verse tus URLs:

```
URL_FORMULARIO_CURSO_1  →  https://forms.gle/abc123...
URL_FORMULARIO_CURSO_2  →  https://www.tuacademia.com/inscripcion-mf1207
URL_FORMULARIO_CURSO_3  →  https://typeform.com/to/xyz789
URL_FORMULARIO_CURSO_4  →  https://www.tuacademia.com/formularios/mf0836
```

Puedes usar:
- Google Forms
- Typeform
- Microsoft Forms
- Tu propio sitio web
- Cualquier plataforma de formularios

## 🖼️ Recursos para Imágenes Gratuitas

### Sitios recomendados (sin necesidad de atribución):

1. **Unsplash** - https://unsplash.com
   - Términos de búsqueda sugeridos:
     - "computer repair" (mantenimiento)
     - "computer assembly" (montaje)
     - "elderly care" (apoyo psicosocial)
     - "solar panels" (fotovoltaica)
     - "professional cooking" (culinaria)
     - "home care" (atención domiciliaria)

2. **Pexels** - https://pexels.com
   - Búsquedas en español también funcionan bien

3. **Pixabay** - https://pixabay.com
   - Gran variedad de imágenes libres

### Optimizar las imágenes:

Antes de usar las imágenes, redimensiónalas a **600x200 píxeles**:

- **Online**: TinyPNG (https://tinypng.com) - Comprime imágenes
- **Online**: Canva (https://canva.com) - Redimensiona gratis
- **Programa**: GIMP (gratuito), Photoshop, etc.

## 📧 Servicios de Email Marketing Recomendados

Para enviar la newsletter profesionalmente:

### Gratuitos (con límites):
1. **Mailchimp** - Hasta 500 contactos gratis
2. **Sendinblue (Brevo)** - Hasta 300 emails/día gratis
3. **MailerLite** - Hasta 1,000 suscriptores gratis

### De pago (para mayor volumen):
1. **SendGrid**
2. **Mailjet**
3. **Constant Contact**

## ⚡ Proceso Rápido (5 Pasos)

1. **Reemplazar 6 URLs** de formularios → 2 minutos
2. **Descargar 6 imágenes** de Unsplash → 5 minutos
3. **Subir imágenes** a tu servidor → 3 minutos
4. **Actualizar contacto** en footer → 1 minuto
5. **Probar** enviándote un email de prueba → 2 minutos

**Total: ≈ 15 minutos** y estarás listo para enviar.

## 🧪 Cómo Probar la Newsletter

### Prueba Local (en navegador):
1. Abre `newsletter-template.html` en Chrome/Firefox
2. Haz clic en todos los botones para verificar los enlaces
3. Redimensiona la ventana para ver el diseño responsive

### Prueba de Email:
1. Envíate un email de prueba a ti mismo
2. Ábrelo en diferentes dispositivos:
   - ✓ Móvil (Gmail app, Mail app)
   - ✓ Tablet
   - ✓ Ordenador (Gmail web, Outlook)
3. Verifica que:
   - Las imágenes se carguen
   - Los botones funcionen
   - El diseño se vea bien

### Herramientas Online:
- **Litmus** (https://litmus.com) - Vista previa en múltiples clientes
- **Mail Tester** (https://mail-tester.com) - Verifica spam score
- **Email on Acid** - Pruebas de renderizado

## ❓ Preguntas Frecuentes

**P: ¿Puedo cambiar los colores?**
R: Sí, busca los códigos de color en el HTML (ej: #667eea, #10b981) y reemplázalos.

**P: ¿Puedo añadir más cursos?**
R: Sí, copia toda una sección de curso (`<tr><td>...tarjeta de curso...</td></tr>`) y pégala debajo.

**P: ¿Las imágenes deben ser exactamente 600x200px?**
R: Es recomendado para mejor rendimiento, pero pueden ser un poco más grandes. El sistema las redimensionará automáticamente.

**P: ¿Puedo editar las descripciones de los cursos?**
R: ¡Por supuesto! Edita el texto dentro de las etiquetas `<p>` de cada curso.

**P: ¿Funciona en todos los clientes de email?**
R: Está optimizada para la mayoría (Gmail, Outlook, Apple Mail, etc.), pero algunos clientes muy antiguos pueden tener limitaciones.

---

**¿Necesitas más ayuda?** Consulta el archivo `README.md` para instrucciones detalladas.
