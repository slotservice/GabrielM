# Mi Votación de los Jugadores - Guía de Uso

Este proyecto contiene el diseño HTML/CSS para mostrar la votación de jugadores del partido Uruguay vs Chile.

## 📁 Estructura de Archivos

```
/
├── index.html              # Archivo HTML principal
├── styles.css              # Estilos CSS del diseño
├── README.md              # Este archivo
└── assets/
    ├── fondo.png          # Imagen de fondo
    ├── logo-coca-cola.svg # Logo de Coca-Cola
    ├── logo-ovacion.svg   # Logo de Ovación
    ├── estrella.svg       # Icono de estrella
    ├── banner-logos.png   # Banner con logos
    └── players/           # Carpeta de fotos de jugadores
        ├── player1.PNG
        ├── player2.PNG
        ├── player3.PNG
        └── player4.PNG
```

## 🚀 Cómo Usar

1. Abre el archivo `index.html` en tu navegador web
2. El diseño se mostrará en la esquina superior izquierda sin márgenes
3. No tiene adaptación responsive (diseño de ancho fijo)

## 🖼️ Cómo Cambiar las Fotos de Jugadores

Las fotos de los jugadores son archivos **independientes** que puedes cambiar fácilmente:

### Método Simple:
1. Ve a la carpeta `assets/players/`
2. Reemplaza los archivos existentes (`player1.PNG`, `player2.PNG`, etc.) con tus nuevas fotos
3. **IMPORTANTE**: Mantén el mismo nombre de archivo
4. **IMPORTANTE**: Usa el mismo tamaño que las fotos originales (aproximadamente 135x120 píxeles)
5. Recarga la página en el navegador

### Recomendaciones para las Fotos:
- **Formato**: PNG o JPG
- **Tamaño recomendado**: 135px de ancho x 120px de alto (o proporción similar)
- **Fondo**: Preferiblemente blanco o transparente (PNG)
- **Recorte**: Centrado en el rostro del jugador
- **Calidad**: Alta resolución para mejor visualización

### Ejemplo:
Si tienes una nueva foto de Darwin Núñez:
1. Recorta la foto a 135x120 píxeles (o tamaño proporcional)
2. Guárdala como `player1.PNG`
3. Copia el archivo a `assets/players/` (reemplaza el existente)
4. Recarga la página - ¡listo!

## ✏️ Cómo Editar los Textos

Todos los textos están en formato **texto editable** (no son imágenes). Para cambiarlos:

### 1. Editar Información del Partido:
Busca en `index.html` la sección `match-info`:

```html
<p class="match-info">Partido <strong>Uruguay – Chile</strong> 15/9/2025</p>
```

Cambia los nombres de equipos y la fecha según necesites.

### 2. Editar Posición del Jugador:
Busca el elemento con clase `position-label`:

```html
<div class="position-label">DELANTERO</div>
```

Opciones comunes:
- DELANTERO
- DEFENSA
- MEDIOCAMPO
- ARQUERO

### 3. Editar Nombre del Jugador:
Busca la sección `player-name`:

```html
<div class="player-name">
    <span class="first-name">DARWIN</span>
    <span class="last-name">NÚÑEZ</span>
</div>
```

Cambia el texto dentro de los `<span>` según el jugador.

### 4. Editar Puntos:
Busca el elemento con clase `points-number`:

```html
<span class="points-number">9</span>
```

Cambia el número según la puntuación del jugador.

## ⭐ Jugador Estrella

El segundo jugador de la primera fila tiene un diseño especial con borde dorado y etiqueta "JUGADOR ESTRELLA ★".

Para cambiar cuál jugador es la estrella:
1. Busca en `index.html` el elemento `<div class="player-card star-player">`
2. Muévelo a la posición del jugador que quieras destacar
3. Asegúrate de incluir todos los elementos especiales (clases `gold` y el `star-badge`)

## 🎨 Personalización de Colores

Los colores principales están definidos en `styles.css`:

- **Fondo verde**: `#0a3d1f`
- **Verde jugador**: `#2d6e3f`
- **Dorado estrella**: `#d4a017` y `#f4d03f`
- **Negro**: `#000000` y `#1a1a1a`

Para cambiar colores, edita estos valores en el archivo CSS.

## 📐 Dimensiones del Diseño

- **Ancho total**: 619px
- **Alto total**: 1101px
- **Tarjeta de jugador**: ~135px de ancho
- **Grid**: 4 columnas x 4 filas
- **Separación**: 15px entre tarjetas

## 🔧 Solución de Problemas

### Las imágenes no se muestran:
- Verifica que las rutas en `index.html` sean correctas
- Asegúrate de que los archivos estén en la carpeta `assets/` y `assets/players/`

### El diseño se ve diferente:
- Asegúrate de que ambos archivos (`index.html` y `styles.css`) estén en la misma carpeta
- Verifica que el navegador esté actualizado

### Las fotos de jugadores se ven distorsionadas:
- Usa fotos con la proporción correcta (aproximadamente 140x160px)
- Si las fotos son de diferente tamaño, ajusta manualmente en CSS

## 💡 Consejos

1. **Mantén una copia de seguridad** de las fotos originales antes de reemplazarlas
2. **Usa nombres consistentes** para los archivos de fotos
3. **Mantén el mismo formato** (PNG/JPG) para todas las fotos
4. **Optimiza las imágenes** para web para una carga más rápida

## 📝 Notas

- Este diseño **NO es responsive** (según especificación del cliente)
- El contenedor está fijado en la **esquina superior izquierda sin márgenes**
- Todos los elementos son **independientes y editables**
- Los textos son **texto real**, no imágenes

---

**Desarrollado por**: [Tu Nombre]  
**Fecha**: Noviembre 2025  
**Cliente**: Gabriel M.

Para soporte o consultas, contacta al desarrollador.

