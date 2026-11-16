- Portafolio personal de Carlos Sehuanes

Este proyecto es mi portafolio personal como estudiante de desarrollo de software
La pagina presenta quien soy, mis habilidades, los trabajos que quiero mostrar, mi proceso de aprendizaje y las formas de contactarme
El objetivo del trabajo fue organizar el contenido y darle un estilo claro y agradable usando HTML y Bootstrap 

- Que se hizo

Primero se organizo la estructura del HTML para que cada parte tuviera un lugar definido

El nombre y el menu quedaron dentro del header, la foto y la presentacion personal quedaron al inicio del main despues aparecen las secciones del portafolio y al final esta el footer

Se agregaron enlaces en el menu para llegar a cada seccion sin salir de la pagina

Luego se aplique un diseño de tarjetas suaves, cada bloque de contenido tiene espacio interior, esquinas redondeadas y una sombra pequeña, los fondos alternan entre marfil, verde suave y arena clara para distinguir las secciones

Las habilidades quedaron separadas en tecnologias y habilidades personales. Cada habilidad se muestra como una etiqueta

El proyecto Rueda Libre tiene un bloque visual con sus iniciales y un enlace a su repositorio

La formacion actual, la ruta de aprendizaje y el horario de estudio quedaron agrupados.

Tambien le di estilo a la experiencia, los enlaces de contacto y el pie de pagina

- Herramientas utilizadas

HTML organiza los titulos, textos, listas, imagenes, enlaces y tablas

Bootstrap aporta las clases para distribuir el contenido, crear tarjetas, botones y espacios y adaptar las columnas a distintos tamaños de pantalla

CSS permite personalizar los colores de Bootstrap para que el portafolio tenga una identidad propia

La pagina es un sitio estatico, el contenido esta escrito directamente en el HTML y no depende de una base de datos ni de un servidor propio

-  Archivos del proyecto

Portafolio/
├── README.md
├── index.html
├── css/
│   └── estilos.css
└── imagenes/
    ├── image.png
    └── Mi.jpeg


[index.html](index.html) contiene toda la estructura y el contenido visible de la pagina

[css/estilos.css](css/estilos.css) contiene la paleta de colores y los ajustes de los botones y la tabla

[imagenes/image.png](imagenes/image.png) es la imagen que se usa actualmente en la presentacion

[imagenes/Mi.jpeg](imagenes/Mi.jpeg) es una foto anterior que conserve en la carpeta.


- Como esta organizada la pagina

    * Cabecera y menu
    
    El header contiene el nombre y el menu principal
    Dentro del header esta el nav con los enlaces de Inicio, Sobre mi, Habilidades, Proyectos, Formacion, Experiencia y Contacto
    Cada enlace apunta al identificador de una seccion. Por ejemplo
    
    <a href="#proyectos">Proyectos</a>
    
    <section id="proyectos">
        <h2>Mis proyectos</h2>
    </section>
    
    
    Al pulsar el enlace el navegador lleva al contenedor de proyectos
    Los identificadores estan en las secciones y no en los titulos.
    
    * Presentacion
    
    Muestra la foto, el nombre completo y una frase sobre el proceso de formacion
    Inclui dos enlaces con apariencia de boton para ver los proyectos o ir al contacto
    La foto actual y sus Las clases de Bootstrap le dan forma circular y recortan la imagen sin deformarla
    
    * Sobre mi
    
    Tiene un espacio para contar mi historia, intereses y objetivos como desarrollador
    
    * Habilidades
    
    El contenido se divide en tecnologias y habilidades personales
    Mostre conocimientos de HTML y CSS, Git y GitHub, ingles y deporte de alto rendimiento
    
    * Proyectos
    
    Actualmente tengo Rueda Libre
    El bloque RL es un elemento visual hecho con HTML y clases de Bootstrap, no es la captura de pantalla del proyecto
    El enlace Visita mi proyecto abre su repositorio en GitHub
    
    * Formacion y aprendizaje
    
    Incluye mi formacion en Riwi y Quick Learning
    Tambien muestra mi ruta de aprendizaje de HTML y CSS, JavaScript, backend y bases de datos
    El horario conserva los dias, temas y horas definidos en el HTML. La tabla esta dentro de un contenedor que permite desplazamiento horizontal si llega a necesitar mas espacio
    
    * Experiencia
    
    Presenta mi informacion actual sobre el bachillerato, el proceso de formacion en software y los conocimientos en construccion
    
    * Contacto y pie de pagina
    
    La seccion de contacto contiene enlaces a GitHub y al correo
    El enlace de correo usa mailto para abrir la aplicacion de correo configurada en el equipo. 
    El footer muestra el nombre, el año y los enlaces finales
    
- Como funcionan las clases principales

Las clases de Bootstrap son nombres que se agregan al atributo class del HTML cada nombre aplica propiedades de CSS que ya vienen preparadas
Varias clases pueden trabajar sobre el mismo elemento. Por ejemplo

<section class="card rounded-4 shadow-sm p-4 mb-4 bg-light">

En este caso cada clase cumple una tarea


card:Crea un contenedor con borde y organiza su contenido en columna 
rounded-4: Redondea las esquinas con un radio de 1rem 
shadow-sm: Agrega una sombra pequeña 
p-4 : Agrega 1.5rem de espacio dentro del contenedor 
mb-4: Agrega 1.5rem de margen debajo del contenedor 
bg-light: Aplica el fondo claro configurado en la paleta 

Con el tamaño habitual 1rem equivale a 16 pixeles, Por eso p-4 deja 24 pixeles de espacio interior y rounded-4 usa esquinas de 16 pixeles
El padding separa el contenido de sus propios bordes, el margin separa un elemento de los elementos que tiene alrededor
La clase container centra el contenido y limita su ancho segun el tamaño de pantalla
La clase row crea una fila para organizar columnas. La clase col-12 ocupa todo el ancho de la fila y col-md-6 ocupa la mitad desde 768 pixeles
Se usan col-md-3 para la foto y col-md-9 para el texto,desde ese mismo tamaño reparten la fila en 25 por ciento y 75 por ciento.En pantallas pequeñas cada bloque ocupa una fila completa
Las clases order-md-1 y order-md-2 cambian el orden visual para colocar el texto antes de la foto en pantallas medianas y grandes
La clase badge da forma de etiqueta a las habilidades. text-wrap permite que una frase larga pase a otra linea y flex-wrap permite que las etiquetas bajen de fila cuando falta espacio
Los enlaces de accion usan btn junto con btn-primary o btn-secondary. btn aporta la forma del boton y las otras clases definen sus colores y estados de interaccion

* Colores y CSS propio

La paleta usa verdes y tonos calidos

Fondo general crema: #fbf7ed 
Verde bosque del menu y botones: #2f513b 
Fondo marfil: #fffdf7 
Fondo verde suave: #e9efdf 
Fondo arena clara: #f6f0e4 
Terracota de enlaces y detalles: #a5492e 


* Como actualizar el contenido si lo en un futuro se quiere actulizar o usar

Para cambiar textos en index.html y busca la seccion que quieres editar.

Para usar otra foto guarda la imagen en la carpeta imagenes y cambia el atributo src del elemento img

Para agregar un proyecto puedes tomar como base el article de Rueda Libre, cambia el nombre y el enlace por los datos reales del nuevo trabajo

Para agregar una fila al horario usa un nuevo tr dentro del tbody. Cada td representa una celda con el dia, el tema o las horas

Para cambiar colores edita las variables de estilos.css, recomiendo cambiar un grupo de colores a la vez y revisar el resultado antes de seguir

Al editar conserva los identificadores de las secciones o actualiza tambien los enlaces del menu que los usan


* Autor

Carlos Esteban Sehuanes Leon

Estudiante de desarrollo de software
