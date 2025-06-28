# Socio.AI - Landing Page

Una landing page moderna con flat design para servicios de marketing automatizado con IA, diseñada específicamente para el mercado argentino.

## 🚀 Características

- **Diseño Flat Moderno**: Interfaz limpia y atractiva con animaciones suaves
- **Responsive**: Optimizada para todos los dispositivos
- **Formulario de Contacto Funcional**: Integrado con EmailJS para envío de emails sin backend
- **Animaciones**: Efectos de scroll y hover para mejor experiencia de usuario
- **SEO Optimizado**: Meta tags y estructura semántica

## 📧 Configuración del Formulario de Contacto

### 1. Crear cuenta en EmailJS

1. Ve a [https://www.emailjs.com](https://www.emailjs.com)
2. Crea una cuenta gratuita
3. Verifica tu email

### 2. Configurar el servicio de email

1. En el dashboard de EmailJS, ve a "Email Services"
2. Haz clic en "Add New Service"
3. Selecciona tu proveedor de email (Gmail, Outlook, etc.)
4. Sigue las instrucciones para conectar tu cuenta
5. Anota el **Service ID** que se genera

### 3. Crear una plantilla de email

1. Ve a "Email Templates"
2. Haz clic en "Create New Template"
3. Usa esta plantilla como base:

```html
Nueva solicitud de auditoría digital

Nombre: {{from_name}}
Email: {{from_email}}
Negocio: {{business_name}}

Fecha: {{date}}
```

4. Anota el **Template ID** que se genera

### 4. Obtener la Public Key

1. Ve a "Account" en el menú lateral
2. Copia tu **Public Key**

### 5. Actualizar el código

En el archivo `index.html`, reemplaza los siguientes valores:

```javascript
// Línea 365 - Public Key
publicKey: 'TU_PUBLIC_KEY_AQUI'

// Línea 395 - Service ID
const serviceID = 'TU_SERVICE_ID_AQUI'

// Línea 396 - Template ID  
const templateID = 'TU_TEMPLATE_ID_AQUI'
```

## 🎨 Personalización

### Colores
Los colores se pueden modificar en las variables CSS al inicio del archivo:

```css
:root {
    --primary: #6366f1;        /* Color principal */
    --primary-dark: #4f46e5;   /* Color principal oscuro */
    --secondary: #f59e0b;      /* Color secundario */
    --accent: #10b981;         /* Color de acento */
    /* ... más variables */
}
```

### Contenido
- **Títulos y textos**: Modifica directamente en el HTML
- **Imágenes**: Reemplaza las URLs de las imágenes con las tuyas
- **Información de contacto**: Actualiza el footer

## 📱 Responsive Design

La página está optimizada para:
- Desktop (1200px+)
- Tablet (768px - 1199px)
- Mobile (< 768px)

## 🚀 Despliegue

### Opción 1: GitHub Pages
1. Sube el código a un repositorio de GitHub
2. Ve a Settings > Pages
3. Selecciona la rama main como fuente
4. Tu sitio estará disponible en `https://tuusuario.github.io/turepo`

### Opción 2: Netlify
1. Ve a [netlify.com](https://netlify.com)
2. Arrastra la carpeta del proyecto
3. Tu sitio se desplegará automáticamente

### Opción 3: Vercel
1. Ve a [vercel.com](https://vercel.com)
2. Conecta tu repositorio de GitHub
3. Vercel detectará automáticamente que es un sitio estático

## 🔧 Estructura del Proyecto

```
landing_autenith/
├── index.html          # Página principal
├── README.md           # Este archivo
└── assets/             # (Opcional) Para imágenes locales
    ├── images/
    └── css/
```

## 📞 Soporte

Si tienes problemas con la configuración:
1. Revisa que todas las claves de EmailJS estén correctamente configuradas
2. Verifica que el servicio de email esté conectado
3. Revisa la consola del navegador para errores

## 📄 Licencia

Este proyecto es de uso libre. Puedes modificarlo y usarlo para tus propios proyectos.

---

**Socio.AI** - Marketing Automatizado para Negocios que Crecen 