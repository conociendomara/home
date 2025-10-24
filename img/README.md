# Imágenes del Municipio Mara

Esta carpeta contiene todas las imágenes locales utilizadas en la aplicación de turismo.

## Estructura de Archivos

### Imágenes de Destinos

Coloca las imágenes de cada destino con los siguientes nombres:

#### Destinos Culturales
- `san-rafael-mojan.jpg` - San Rafael de El Moján (Plaza & Iglesia)
- `puente-guajira.jpg` - Puente Guajira Venezolana (Río Limón)
- `juyasirrain.jpg` - Juyasirrain (Sitio arqueológico)

#### Destinos Naturales (Floras y Faunas)
- `laguna-sinamaica.jpg` - Laguna de Sinamaica
- `lago-maracaibo.jpg` - Orillas del Lago de Maracaibo
- `serranias-senderos.jpg` - Serranías y Senderos
- `medanos-mara.jpg` - Los Médanos de Mara
- `acantilados-nigale.jpg` - Los Acantilados Nigale
- `cerro-san-andres.jpg` - El Cerro San Andrés
- `rio-cachiri.jpg` - El Río Cachiri

## Especificaciones Técnicas

### Formato Recomendado
- **Formato**: JPG o PNG
- **Resolución**: 400x300px (4:3) o 400x225px (16:9)
- **Tamaño**: Máximo 200KB por imagen para carga rápida
- **Calidad**: 80-90% para balance entre calidad y tamaño

### Optimización
- **Compresión**: Usar herramientas como TinyPNG o ImageOptim
- **Responsive**: Las imágenes se escalan automáticamente
- **Lazy Loading**: Implementado para mejor rendimiento

## Cómo Agregar Imágenes

1. **Toma o descarga** las imágenes de cada destino
2. **Renombra** cada imagen según la lista de arriba
3. **Optimiza** el tamaño y calidad
4. **Coloca** en esta carpeta `img/`
5. **Verifica** que se muestren correctamente en la aplicación

## Fallback de Imágenes

Si una imagen no se puede cargar, la aplicación muestra:
- Un icono SVG genérico
- Un mensaje de error en la consola
- La aplicación continúa funcionando normalmente

## Estructura de URLs

Las imágenes se cargan desde:
```
img/san-rafael-mojan.jpg
img/puente-guajira.jpg
img/laguna-sinamaica.jpg
...
```

## Ejemplo de Uso

```html
<img src="img/san-rafael-mojan.jpg" 
     alt="San Rafael de El Moján" 
     onerror="this.src='data:image/svg+xml;base64,...'">
```

## Notas Importantes

- **Nombres de archivo**: Deben coincidir exactamente con los especificados
- **Rutas relativas**: Las imágenes se cargan desde la carpeta `img/`
- **Compatibilidad**: Funciona en todos los navegadores modernos
- **Responsive**: Se adaptan automáticamente a diferentes tamaños de pantalla
- **Carga optimizada**: Solo se cargan cuando son necesarias

## Herramientas Recomendadas

### Para Optimizar Imágenes
- **TinyPNG**: https://tinypng.com/
- **ImageOptim**: https://imageoptim.com/
- **Squoosh**: https://squoosh.app/

### Para Redimensionar
- **GIMP**: Software gratuito
- **Photoshop**: Profesional
- **Canva**: Online, fácil de usar

## Estructura de Carpetas

```
img/
├── san-rafael-mojan.jpg
├── puente-guajira.jpg
├── laguna-sinamaica.jpg
├── lago-maracaibo.jpg
├── serranias-senderos.jpg
├── medanos-mara.jpg
├── acantilados-nigale.jpg
├── cerro-san-andres.jpg
├── rio-cachiri.jpg
├── juyasirrain.jpg
└── README.md
```

## Troubleshooting

### Imagen no se muestra
1. Verifica que el nombre del archivo coincida exactamente
2. Asegúrate de que el archivo esté en la carpeta `img/`
3. Verifica que el archivo no esté corrupto
4. Revisa la consola del navegador para errores

### Imagen se ve pixelada
1. Usa una imagen de mayor resolución
2. Verifica que el formato sea JPG o PNG
3. Optimiza la compresión

### Carga lenta
1. Reduce el tamaño del archivo
2. Optimiza la compresión
3. Usa formato JPG para fotos
