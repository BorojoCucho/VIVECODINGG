# ETS Infoplus - Plataforma Educativa sobre Salud Sexual

Una plataforma web integral que combina contenido educativo gamificado con herramientas de autoevaluación de síntomas y geolocalización de centros médicos especializados para promover la prevención de ETS, reducir la desinformación y facilitar el acceso a atención médica confiable.

## Características Principales

- **📚 Centro Educativo**: Información detallada sobre diferentes tipos de ETS, síntomas, transmisión y tratamientos
- **🎮 Gamificación**: Quiz interactivos para aprender mientras se divierten
- **🩺 Autoevaluación de Síntomas**: Herramienta para evaluar posibles riesgos de salud
- **📍 Geolocalización de Centros Médicos**: Encuentra centros especializados cercanos a tu ubicación
- **🛡️ Consejos de Prevención**: Estrategias efectivas para prevenir ETS
- **💬 Información Confiable**: Contenido basado en evidencia científica

## Equipo de Desarrollo

- Juan Jose Restrepo Alvarez
- Joseph Alexander Morales Cardona
- Emanuel Granados Pulgarin
- Samuel Torres Atehortua
- Jacobo Morales Londoño

## Estructura del Proyecto

```
ets-infoplus/
├── client/                 # Frontend React
│   ├── src/
│   │   ├── pages/         # Páginas de la aplicación
│   │   │   ├── Home.tsx
│   │   │   ├── Education.tsx
│   │   │   ├── SelfAssessment.tsx
│   │   │   ├── MedicalCenters.tsx
│   │   │   ├── Quiz.tsx
│   │   │   └── About.tsx
│   │   ├── components/    # Componentes reutilizables
│   │   ├── App.tsx        # Enrutador principal
│   │   └── index.css      # Estilos globales
│   └── public/
│       └── images/        # Imágenes educativas
├── shared/                # Constantes compartidas
│   └── const.ts          # Datos de ETS, preguntas, centros médicos
└── README.md             # Este archivo
```

## Instalación y Desarrollo

### Requisitos Previos

- Node.js 18+ 
- npm o pnpm

### Pasos de Instalación

1. **Clonar el repositorio**
```bash
git clone https://github.com/tu-usuario/ets-infoplus.git
cd ets-infoplus
```

2. **Instalar dependencias**
```bash
pnpm install
```

3. **Ejecutar el servidor de desarrollo**
```bash
pnpm dev
```

El servidor estará disponible en `http://localhost:3000`

## Despliegue

### Despliegue en Netlify

1. **Conectar el repositorio a Netlify**
   - Ir a [Netlify](https://netlify.com)
   - Conectar tu repositorio de GitHub
   - Configurar los siguientes parámetros:
     - **Build command**: `pnpm build`
     - **Publish directory**: `dist`

2. **Desplegar**
   - Netlify construirá y desplegará automáticamente en cada push a main

### Despliegue en GitHub Pages

1. **Crear rama gh-pages**
```bash
git checkout --orphan gh-pages
git rm -rf .
```

2. **Construir el proyecto**
```bash
pnpm build
```

3. **Copiar archivos a gh-pages**
```bash
cp -r dist/* .
git add .
git commit -m "Deploy to GitHub Pages"
git push origin gh-pages
```

4. **Configurar en GitHub**
   - Ir a Settings → Pages
   - Seleccionar `gh-pages` como rama de origen

## Páginas Principales

### 1. Inicio (/)
- Presentación de la plataforma
- Características principales
- Consejos de prevención
- Llamadas a la acción

### 2. Educación (/educacion)
- Información sobre 6 tipos de ETS
- Detalles de síntomas, transmisión y tratamiento
- Información general sobre ETS

### 3. Autoevaluación (/autoevaluacion)
- Evaluador interactivo de síntomas
- Clasificación de riesgo (bajo, moderado, alto)
- Recomendaciones basadas en síntomas

### 4. Centros Médicos (/centros-medicos)
- Listado de centros especializados
- Geolocalización (requiere permiso del usuario)
- Distancia calculada automáticamente
- Información de contacto y servicios

### 5. Quiz (/quiz)
- 5 preguntas sobre prevención de ETS
- Retroalimentación inmediata
- Puntuación final y análisis

### 6. Acerca de (/acerca-de)
- Información sobre el proyecto
- Misión y objetivos
- Equipo de desarrollo
- Valores de la plataforma

## Tecnologías Utilizadas

- **Frontend**: React 19, TypeScript, Tailwind CSS
- **Enrutamiento**: Wouter
- **Componentes UI**: shadcn/ui
- **Build Tool**: Vite
- **Gestor de Paquetes**: pnpm

## Características de Seguridad

- ✅ Información confidencial del usuario (no se almacena)
- ✅ Geolocalización opcional (requiere consentimiento)
- ✅ Sin recopilación de datos personales
- ✅ Contenido educativo sin diagnósticos médicos

## Notas Importantes

⚠️ **Descargo de Responsabilidad**: Esta plataforma es educativa y no reemplaza la consulta médica profesional. Siempre consulta con un profesional de salud calificado para diagnóstico y tratamiento.

## Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## Licencia

Este proyecto está bajo la licencia MIT. Ver el archivo `LICENSE` para más detalles.

## Contacto

Para preguntas o sugerencias sobre la plataforma, por favor contacta al equipo de desarrollo.

---

**Última actualización**: Octubre 2024
**Versión**: 1.0.0

