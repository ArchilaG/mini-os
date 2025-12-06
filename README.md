# Escritorio Windows Vista

Este proyecto es una recreación visual del escritorio de Windows Vista usando solo HTML y CSS.

## Integrantes del grupo

- Carlos Andres Monterrosa Gallego (index)
- Andrés Mauricio Hidrobo Escalona (calculadora)

## Qué se hizo

Se creó una interfaz de escritorio que simula el aspecto de Windows Vista, incluyendo:

- Un escritorio con fondo degradado azul característico de Vista
- Iconos de aplicaciones en la parte superior izquierda (Galería, Calculadora y Buscador)
- Calculadora: Simula la visivilidad de una calculadora con botones que cambian de tamaño ya sea al pasar el mouse por encima o dando click para simular ser botones funcionales
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
Index hecho por Santiago Manuel Archila Guarnizo

## Visualizador de fotos de Windows (Simulación UI)

Este proyecto es una recreación visual de la interfaz de usuario del Visualizador de fotos de Windows (Windows Photo Viewer), específicamente simulando el estilo de las versiones de Windows Vista o Windows 7. Se ha construido utilizando exclusivamente HTML y CSS para replicar la apariencia de la ventana de la aplicación.

# Qué se hizo

Se ha simulado la estructura completa y el estilo visual de la ventana del Visualizador de fotos, incluyendo:

    Barra de Título: La barra superior con el fondo gris/azul claro, el texto del título, y los botones de control de la ventana (Minimizar, Maximizar/Restaurar y Cerrar), incluyendo el estilo distintivo del botón Cerrar (X) en rojo.

    Barra de Menú: La barra debajo del título con opciones como "Archivo", "Imprimir", etc., y el botón de ayuda (?).

    Área de Imagen (Área de Trabajo): El fondo principal en azul muy claro (#EAF2FC) que simula el área de la aplicación.

    Carrusel de Imágenes: Un contenedor central con scroll horizontal que permite simular la navegación entre varias imágenes.

    Marco de Imagen: El estilo que enmarca cada imagen dentro del carrusel con un borde y una sombra para simular el papel fotográfico o el marco de la aplicación.

    Barra Inferior (Footer): La barra de herramientas inferior con el color azul oscuro característico de la interfaz de Windows Vista/7.

## Estructura y Archivos

El proyecto consta de dos archivos principales:
Archivo	Función
gallery.html	Estructura principal de la ventana (Barra de título, Menús, Área de imagen y Footer).
galleystyles.css	Todos los estilos para replicar el aspecto visual de la aplicación y la funcionalidad del carrusel.

## Técnicas CSS y Componentes Clave

El diseño se basa fuertemente en Flexbox para asegurar que los componentes de la ventana se organicen correctamente de arriba a abajo y que el área de imagen ocupe todo el espacio disponible.
Organización de la Ventana (.main-container)

    Se usa display: flex; con flex-direction: column; para apilar verticalmente la barra de título, la barra de menú, el área central y la barra inferior.

    El elemento .image-area tiene flex-grow: 1; para ocupar todo el espacio vertical que dejan las barras de título, menú y pie de página.

Simulación de Carrusel (.carousel-container)

El carrusel central se logra con las siguientes propiedades CSS en el contenedor:

    display: flex; y overflow-x: scroll; para permitir el desplazamiento horizontal.

    scroll-snap-type: x mandatory; y scroll-snap-align: center; en las imágenes para forzar que el desplazamiento se detenga perfectamente centrado en cada imagen, simulando una interfaz de carrusel limpia.

    Se oculta la barra de desplazamiento nativa con ::-webkit-scrollbar para una apariencia más limpia.

Estilo Aero Glass y Componentes de Ventana

    Colores: Se utilizan colores específicos (#DAE4F0, #EAF2FC, #5D93D0) para replicar la paleta de Windows.

    Botón de Cerrar (#close): Se le da el estilo final de Windows con background-color: #E81123; (rojo).

    Marco de Imagen: Se utiliza una combinación de border: 1px solid #C4C4C4; y box-shadow: 0 0 5px rgba(0, 0, 0, 0.2); para crear el efecto de marco y profundidad.
