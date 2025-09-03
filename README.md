# Ronny.dev - Blog Técnico de Ciberseguridad

Blog técnico personal sobre ingeniería en sistemas, ciberseguridad y pentesting, desarrollado con Next.js y TailwindCSS.

## 🚀 Características

- **Diseño "Hacker Elegante"**: Estilo terminal moderno con paleta de colores ciberseguridad
- **Blog Completo**: Sistema de artículos con búsqueda, filtros y categorías
- **Componentes UI**: Terminal cards, bloques de código, tags y más
- **Responsive**: Optimizado para mobile, tablet y desktop
- **SEO Ready**: Meta tags, sitemap y estructura optimizada

## 🛠️ Stack Tecnológico

- **Framework**: Next.js 13+ con App Router
- **Estilos**: TailwindCSS + CSS Variables
- **UI**: shadcn/ui + componentes personalizados
- **Tipografías**: Inter (contenido) + JetBrains Mono (código)
- **Iconos**: Lucide React

## 🎨 Paleta de Colores

```css
--bg-primary: #0B0F14;     /* Fondo principal */
--bg-secondary: #151922;   /* Fondo secundario */
--bg-card: #1A1F2E;       /* Fondo tarjetas */
--text-primary: #E6F1FF;   /* Texto principal */
--text-secondary: #94A3B8; /* Texto secundario */
--accent-green: #00FF7F;   /* Verde terminal */
--accent-cyan: #5EEAD4;    /* Cian */
--border-primary: #334155; /* Bordes */
```

## 📁 Estructura del Proyecto

```
├── app/                    # Pages (App Router)
│   ├── blog/              # Blog pages
│   ├── proyectos/         # Projects page
│   ├── recursos/          # Resources page
│   ├── about/             # About page
│   └── contacto/          # Contact page
├── components/            # Componentes reutilizables
│   ├── layout/           # Layout components
│   └── ui/               # UI components
├── data/                 # Data estática (posts, projects)
├── lib/                  # Utilidades y constantes
└── types/               # TypeScript interfaces
```

## 🚀 Instalación y Desarrollo

### Prerrequisitos
- Node.js 18+
- npm o yarn

### Instalación

```bash
# Clonar el repositorio
git clone https://github.com/ronny/blog-ciberseguridad.git
cd blog-ciberseguridad

# Instalar dependencias
npm install

# Ejecutar en modo desarrollo
npm run dev
```

La aplicación estará disponible en `http://localhost:3000`

### Scripts Disponibles

```bash
npm run dev          # Servidor de desarrollo
npm run build        # Build para producción
npm run start        # Servidor de producción
npm run lint         # Linter ESLint
```

## 📝 Agregar Contenido

### Nuevo Post de Blog

1. Editar `data/blog-posts.ts`
2. Agregar nuevo objeto `BlogPost` con toda la información
3. El contenido va en formato string con markdown básico

### Nuevo Proyecto

1. Editar `data/projects.ts`
2. Agregar nuevo objeto `Project`
3. Incluir tecnologías, links y descripción

### Nuevo Recurso

1. Editar `data/resources.ts`
2. Agregar nuevo objeto `Resource`
3. Categorizar correctamente

## 🎯 Componentes Principales

### TerminalCard
Tarjeta con estilo terminal, header con botones de semáforo.

### CodeBlock
Bloque de código con highlighting, numeración de líneas y botón copiar.

### PostCard
Tarjeta de artículo con meta información, tags y link de lectura.

### Search
Componente de búsqueda en vivo con icono y botón limpiar.

### Tag
Etiquetas con diferentes variantes y tamaños.

## 🚀 Despliegue

### Vercel (Recomendado)

```bash
# Build del proyecto
npm run build

# Deploy a Vercel
npx vercel --prod
```

### Netlify

```bash
# Build del proyecto
npm run build

# Deploy a Netlify
npx netlify deploy --prod --dir=out
```

## 📊 SEO y Analytics

El proyecto incluye:
- Meta tags optimizados
- Open Graph para redes sociales
- Estructura semántica HTML5
- Sitemap automático (Next.js)

Para analytics, agregar tu código en `app/layout.tsx`:

```typescript
// Google Analytics
import { GoogleAnalytics } from '@next/third-parties/google'

// En el return del layout:
<GoogleAnalytics gaId="GA_MEASUREMENT_ID" />
```

## 🔒 Nota Ética

Todo el contenido es educativo y no fomenta actividades ilegales. El objetivo es promover mejores prácticas de seguridad y educación en ciberseguridad.

## 📄 Licencia

MIT License - ver archivo LICENSE para más detalles.

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature
3. Commit tus cambios
4. Push a la rama
5. Abre un Pull Request

---

**Desarrollado con ❤️ por [Ronny](https://github.com/ronny)**