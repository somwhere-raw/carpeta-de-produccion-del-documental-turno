# Prototipo del libro TURNO

Este prototipo contiene:

- `index.html`: visor principal.
- `libro.pdf`: PDF de seis páginas usado en la prueba.
- `vendor/`: lector PDF incluido localmente; no depende de una biblioteca externa.
- `vista-previa.png` y `vista-movil.png`: comprobaciones visuales.

## Funciones incluidas

- Cambio de página completamente instantáneo, sin animaciones.
- Apertura inicial con una hoja negra `TURNO` a la izquierda y la portada a la derecha.
- Pliegos de dos páginas en escritorio y hoja de cierre negra cuando el contenido termina en página impar.
- Navegación directa: clic en la hoja izquierda para retroceder y en la derecha para avanzar, sin flechas visibles.
- Flechas izquierda y derecha del teclado.
- Deslizamiento táctil en móvil.
- Interfaz animada en una barra lateral izquierda en escritorio y superior en móvil vertical.
- Los botones `Índice` y `Páginas` abren y cierran sus propios paneles; no se utilizan cruces de cierre.
- Panel de miniaturas superpuesto, sin títulos auxiliares y sin redimensionar el libro; permanece abierto hasta pulsar nuevamente `Páginas`.
- Un clic fuera de `Índice` o `Páginas` cierra el panel abierto sin ejecutar la navegación de la hoja situada detrás.
- En pantalla completa, el cajón extendido se guarda completamente debajo de la barra principal antes de que esta pueda retirarse; si el cursor continúa sobre la barra, permanece visible.
- Un clic en una zona vacía de la barra principal cierra únicamente el cajón extendido y conserva la barra mientras el cursor permanezca allí.
- Pantalla completa real: las hojas tocan el borde superior y llegan hasta la franja inferior; la barra lateral reaparece al llevar el puntero al borde izquierdo.
- Contador dentro de una franja negra mínima en el borde inferior.
- Enlaces externos clicables y táctiles en la página de referencias.

La portada no forma parte de la numeración. La página posterior a la portada se muestra como página 1.

La página de referencias tiene cuatro direcciones únicas. Dos ya estaban incorporadas en el PDF; las otras dos fueron añadidas como zonas interactivas en `index.html`.

## Publicación

La carpeta puede publicarse directamente en GitHub Pages. El archivo de entrada debe permanecer con el nombre `index.html` y el PDF con el nombre `libro.pdf`.

El prototipo también puede abrirse localmente con doble clic en `index.html`. En ese modo utiliza las imágenes preparadas de la carpeta `pages/`; al publicarse en GitHub Pages utiliza directamente `libro.pdf`, renderiza únicamente las páginas visibles y vuelve a calcular la resolución al cambiar el tamaño o activar pantalla completa.
