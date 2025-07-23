# ETHALUX - Sitio Web Corporativo

## Descripción
Sitio web moderno y responsive para ETHALUX, una tienda virtual de productos de bienestar, cuidado personal y hogar con presencia regional en Colombia, Chile, Panamá y Ecuador.

## Características Principales

### 🌟 Funcionalidades
- **Selector de País**: Cambia automáticamente productos y precios según el país seleccionado
- **Catálogo de Productos**: Productos organizados por categorías (Cuidado Personal, Hogar, Bienestar)
- **Diseño Responsive**: Optimizado para desktop, tablet y móvil
- **Navegación Intuitiva**: Menú fijo con navegación suave entre secciones
- **Formulario de Contacto**: Sistema de contacto funcional por país

### 🎨 Diseño
- **Paleta de Colores**: Dorado, blanco y tonos tierra
- **Tipografía**: Moderna y legible
- **Animaciones**: Transiciones suaves y efectos hover
- **Imágenes**: Assets optimizados para web

### 🌍 Cobertura Regional
- **Colombia**: Productos con café, aloe vera y ingredientes andinos
- **Chile**: Rosa mosqueta, quinoa y productos patagónicos  
- **Panamá**: Coco tropical, palo santo y artesanías locales
- **Ecuador**: Cacao ceremonial, arcilla volcánica y textiles andinos

## Tecnologías Utilizadas

- **React 18**: Framework principal
- **Vite**: Build tool y dev server
- **Tailwind CSS**: Framework de estilos
- **Lucide React**: Iconos
- **shadcn/ui**: Componentes UI
- **Framer Motion**: Animaciones (preparado)

## Estructura del Proyecto

```
ethalux-website/
├── public/                 # Archivos estáticos
├── src/
│   ├── assets/            # Imágenes y recursos
│   │   ├── ethalux_images/
│   │   │   ├── wellness/
│   │   │   ├── personal_care/
│   │   │   └── home/
│   │   └── ethalux_logo.png
│   ├── components/        # Componentes React
│   │   ├── ui/           # Componentes UI base
│   │   ├── Header.jsx
│   │   ├── Hero.jsx
│   │   ├── About.jsx
│   │   ├── Products.jsx
│   │   ├── Contact.jsx
│   │   └── Footer.jsx
│   ├── data/
│   │   └── products.js   # Base de datos de productos
│   ├── App.jsx           # Componente principal
│   ├── App.css          # Estilos personalizados
│   └── main.jsx         # Punto de entrada
├── dist/                # Build de producción
└── package.json
```

## Instalación y Desarrollo

### Prerrequisitos
- Node.js 18+
- pnpm (recomendado) o npm

### Instalación
```bash
# Clonar el repositorio
git clone <repository-url>
cd ethalux-website

# Instalar dependencias
pnpm install

# Iniciar servidor de desarrollo
pnpm run dev

# Abrir en el navegador
# http://localhost:5173
```

### Scripts Disponibles
```bash
# Desarrollo
pnpm run dev          # Servidor de desarrollo
pnpm run dev --host   # Servidor accesible desde red local

# Producción
pnpm run build        # Crear build de producción
pnpm run preview      # Previsualizar build de producción

# Utilidades
pnpm run lint         # Linter de código
```

## Despliegue

### Build de Producción
```bash
pnpm run build
```
Los archivos optimizados se generan en la carpeta `dist/`

### Opciones de Despliegue
- **Netlify**: Arrastra la carpeta `dist/` o conecta el repositorio
- **Vercel**: Conecta el repositorio GitHub
- **GitHub Pages**: Sube el contenido de `dist/` a la rama gh-pages
- **Servidor Web**: Sube el contenido de `dist/` a tu servidor

### Variables de Entorno (Futuras)
```env
VITE_API_URL=https://api.ethalux.com
VITE_CONTACT_EMAIL=contacto@ethalux.com
```

## Personalización

### Colores de Marca
Los colores están definidos en `src/App.css`:
```css
:root {
  --primary: oklch(0.65 0.15 85);     /* Dorado */
  --secondary: oklch(0.85 0.05 65);   /* Beige */
  --accent: oklch(0.75 0.08 45);      /* Terracota */
}
```

### Productos por País
Edita `src/data/products.js` para:
- Agregar nuevos productos
- Modificar precios
- Cambiar descripciones
- Actualizar imágenes

### Contenido
- **Textos**: Edita directamente en los componentes
- **Imágenes**: Reemplaza archivos en `src/assets/`
- **Logo**: Reemplaza `src/assets/ethalux_logo.png`

## Funcionalidades Futuras

### Próximas Implementaciones
- [ ] Carrito de compras funcional
- [ ] Integración con pasarela de pagos
- [ ] Sistema de usuarios y autenticación
- [ ] Panel de administración
- [ ] Blog de bienestar
- [ ] Sistema de reviews
- [ ] Integración con CRM
- [ ] Analytics y tracking

### Mejoras Técnicas
- [ ] PWA (Progressive Web App)
- [ ] Optimización SEO avanzada
- [ ] Lazy loading de imágenes
- [ ] Caché de productos
- [ ] Internacionalización (i18n)
- [ ] Tests automatizados

## Soporte y Mantenimiento

### Contacto Técnico
- **Desarrollador**: Manus AI
- **Fecha de Creación**: Julio 2025
- **Versión**: 1.0.0

### Actualizaciones
- Revisar dependencias mensualmente
- Actualizar contenido de productos según necesidades
- Monitorear performance y métricas de usuario

## Licencia
Todos los derechos reservados - ETHALUX 2025

