# Videos Temáticos del Municipio Mara

Esta carpeta contiene los archivos de video para la aplicación de turismo, incluyendo videos temáticos que se muestran al seleccionar filtros específicos.

## Estructura de archivos

### Video Principal
- `mara-promocional.mp4` - Video principal del municipio (formato MP4)
- `mara-promocional.webm` - Video principal (formato WebM)
- `mara-promocional.ogg` - Video principal (formato OGG)

### Videos Temáticos

#### Flora y Fauna (Filtro "Floras y faunas")
- `flora-fauna-mara.mp4` - Video sobre biodiversidad marense (formato MP4)
- `flora-fauna-mara.webm` - Video sobre biodiversidad (formato WebM)
- `flora-fauna-mara.ogg` - Video sobre biodiversidad (formato OGG)

#### Cultura (Filtro "Cultura")
- `cultura-mara.mp4` - Video sobre tradiciones culturales (formato MP4)
- `cultura-mara.webm` - Video sobre tradiciones (formato WebM)
- `cultura-mara.ogg` - Video sobre tradiciones (formato OGG)

## Cómo Funciona

1. **Video Principal**: Se muestra en la sección principal de la aplicación
2. **Videos Temáticos**: Se muestran automáticamente cuando el usuario selecciona:
   - **"Floras y faunas"** → Muestra video sobre biodiversidad
   - **"Cultura"** → Muestra video sobre tradiciones culturales
   - **Otros filtros** → Oculta el video temático

## Especificaciones Técnicas

### Resolución Recomendada
- **Ancho**: 1280px (HD) o 1920px (Full HD)
- **Alto**: 720px (HD) o 1080px (Full HD)
- **Relación de aspecto**: 16:9

### Duración Recomendada
- **Videos temáticos**: 1-3 minutos
- **Video principal**: 2-5 minutos

### Tamaño de Archivo
- **Máximo**: 50MB por archivo para carga rápida
- **Recomendado**: 20-30MB por archivo

## Formatos Soportados

### MP4 (Principal)
- **Códec**: H.264
- **Ventaja**: Máxima compatibilidad
- **Uso**: Navegadores modernos

### WebM (Opcional)
- **Códec**: VP9 o VP8
- **Ventaja**: Mejor compresión
- **Uso**: Navegadores que lo soporten

### OGG (Opcional)
- **Códec**: Theora
- **Ventaja**: Compatibilidad con navegadores antiguos
- **Uso**: Fallback para navegadores antiguos

## Cómo Subir a GitHub

1. **Sube los archivos** a esta carpeta `videos/`
2. **GitHub Límite**: 100MB por archivo
3. **Si el archivo es muy grande**:
   - Comprime el video
   - Usa Git LFS (Large File Storage)
   - Sube a un servicio de hosting externo

## Estructura de URLs

Los videos se cargan desde:
```
videos/flora-fauna-mara.mp4
videos/cultura-mara.mp4
videos/mara-promocional.mp4
```

## Personalización

Para cambiar los videos o agregar nuevos temas:

1. **Edita** la función `showThemeVideo()` en `TURISMO.html`
2. **Modifica** el objeto `videoConfig` con las nuevas rutas
3. **Agrega** los archivos de video correspondientes

## Ejemplo de Uso

```javascript
const videoConfig = {
    'montana': {
        title: '🌿 Flora y Fauna de Mara',
        desc: 'Descubre la biodiversidad única...',
        mp4: 'videos/flora-fauna-mara.mp4',
        webm: 'videos/flora-fauna-mara.webm',
        ogg: 'videos/flora-fauna-mara.ogg'
    }
};
```

## Notas Importantes

- Los videos se cargan automáticamente cuando se selecciona el filtro
- Si un video no se puede cargar, se muestra un mensaje de error
- Los controles de reproducción están habilitados
- Los videos tienen un poster (imagen de portada) personalizado
- El sistema es responsive y funciona en móviles