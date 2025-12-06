Index hecho por Carlos Andres Monterrosa Gallego

# Escritorio Windows Vista

Este proyecto es una recreación visual del escritorio de Windows Vista usando solo HTML y CSS.

## Qué se hizo

Se creó una interfaz de escritorio que simula el aspecto de Windows Vista, incluyendo:

- Un escritorio con fondo degradado azul característico de Vista
- Iconos de aplicaciones en la parte superior izquierda (Galería, Calculadora y Buscador)
- Una barra de tareas en la parte inferior con efecto de transparencia
- Botón de inicio con estilo Aero Glass
- Reloj en la barra de tareas
- Pantalla de carga animada que aparece al inicio
- Spinner de carga con animación de rotación
- Menú de inicio que se despliega al pasar el mouse sobre el botón

## Por qué se usó cada tecnología

**HTML:** Se usó para estructurar todos los elementos del escritorio. Cada componente (iconos, barra de tareas, menú) es un elemento HTML organizado de forma jerárquica.

**CSS:** Se utilizó para dar el estilo visual característico de Windows Vista. Incluye degradados para el fondo, transparencias con rgba para simular el efecto Aero Glass, flexbox para organizar los iconos, y animaciones para la pantalla de carga y efectos hover.

**JavaScript:** Solo se usa un pequeño script para reproducir el sonido de inicio cuando carga la página.

## Estructura del proyecto

- `index.html` - Archivo principal con la estructura del escritorio
- `styles.css` - Todos los estilos visuales
- `imagenes/` - Iconos de las aplicaciones
- `sonidos/` - Sonido de inicio de Windows
- `apps/` - Páginas de las aplicaciones

## Técnicas CSS utilizadas

- Degradados lineales para el fondo
- Transparencias con rgba para efectos de cristal
- Flexbox para organizar iconos y elementos de la barra
- Position fixed para mantener la barra de tareas siempre visible
- Animaciones keyframes para la pantalla de carga y el spinner
- Hover effects para interactividad sin JavaScript
- Sombras y bordes para dar profundidad

-----------------------------------------------------------------------
