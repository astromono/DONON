# DONON
DONON es un acrónimo de Diseño Óptico No Ortodoxo-Normativo

Donon pretende ser un programade diseño de sistemas ópticos
    Trata de ser un paquete de diseño de sistemas ópticos pensado desde otro punto de vista.

    Para empezar pretendemos que los espacios o espesores se cuenten desde la superficie actual a la anterior no como la normativa ortodoxa hasta ahora en que todos cuentan la distancia, espesor o espacia a la superficie posterior o siguiente. Esto viene motivado por la idea de trabajar con elementos o conjunto de elementos ópticos que se pueden insertar u ocultar del sistema y que son ellos los que marcan la posicion para la que estan definidos.

    Es no ortodoxasamente normativo porque al configurarse como bloques permite trabajar con cada bloque individualmente o mezclando distintas combinacionesde ellos. ¿Por qué? Pues porque en los instrumentos actuales se montan distintas combinaciones de sistemas que ejecutan tareas diversas y no hay motivo para tener sistemas independientes a la hora de evaluar su funcionalidad. Ruedas de colimadores, ruedas de camaras, ruedas de filtros, ruedas de grismas, cajas negras, etc. Muchas de ellas podrian ser multi-configuraciones pero de hecho a veces cada bloque puede requerir su propia multi-configuración. Todos tendremos ejemplos, ¿uno? Un espectrógrafo trabajando en multiórden y un sistema de rueda de filtros que selecciona una banda de las varias superpuestas y que requiere otra con grismas o prismas que aumenten la dispersion y puedan recentrar una banda ligeramente descentrada a la salida del espectrógrafo.

    Tampoco es una tabla de datos, es, un programa con constantes y variables estructuradas para que las rutinas que van detrás puedan compartir valores que puedan ser cambiados o multivalorados en una cierta configuración o bloque distintos de otros.

    Inicialmente pretendemos arrancar en Python pero estamos valorando la implementación directamente en Julia y solo recurrir a python para las interfaces graficas y de interacción.

    
