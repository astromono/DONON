# DONON
DONON es un acrónimo de Diseño Óptico No Ortodoxo-Normativo

Donon pretende ser o trata de ser un paquete de diseño de sistemas ópticos pensado desde otro punto de vista.

   Para empezar pretendemos que los espacios o espesores se cuenten desde la superficie actual a la anterior no como la normativa ortodoxa hasta ahora en que todos cuentan la distancia, espesor o espacia a la superficie posterior o siguiente. Esto viene motivado por la idea de trabajar con elementos o conjunto de elementos ópticos que se pueden insertar u ocultar del sistema y que son ellos los que marcan la posicion para la que estan definidos.

   Es no ortodoxasamente normativo porque al configurarse como bloques permite trabajar con cada bloque individualmente o mezclando distintas combinacionesde ellos. ¿Por qué? Pues porque en los instrumentos actuales se montan distintas combinaciones de sistemas que ejecutan tareas diversas y no hay motivo para tener sistemas independientes a la hora de evaluar su funcionalidad. Ruedas de colimadores, ruedas de camaras, ruedas de filtros, ruedas de grismas, cajas negras, etc. Muchas de ellas podrian ser multi-configuraciones pero de hecho a veces cada bloque puede requerir su propia multi-configuración. Todos tendremos ejemplos, ¿uno? Un espectrógrafo trabajando en multiórden y un sistema de rueda de filtros que selecciona una banda de las varias superpuestas y que requiere otra con grismas o prismas que aumenten la dispersion y puedan recentrar una banda ligeramente descentrada a la salida del espectrógrafo.

   Tampoco es una tabla de datos, es, un programa con constantes y variables estructuradas para que las rutinas que van detrás puedan compartir valores que puedan ser cambiados o multivalorados en una cierta configuración o bloque distintos de otros.

   Inicialmente pretendemos arrancar en Python pero estamos valorando la implementación directamente en Julia y sólo recurrir a python para las interfaces gráficas y de interacción.

Las ultimas semanas hemos estado valorando crear una interfaz de usuario y rutinas de apoyo para poder interactuar con varios proyectos de diseño óptico abiertos en la red como Optiland, RayTracing, RayOptics, Optics-Workbench, Pyrate, PyrayT, etc. 
El planteamiento es aprovechar las distintas capacidades que ofrece cada uno para el tratamiento de trazado de rayos manipulacion de datos y optimizaciones por rayo o por frente de onda y que ya estan desarrolladas y probadas en cada uno de los paquetes. 

Las principales dificultades de este tipo de trabajo es la compatibilidad del manejo de datos. Empezando por la propia filosofia de nuestro objetivo. Primero el cambio de espesores a la superficie siguiente. Seguido de la idea de empaquetamiento de subsistemas y sobre todo la no secuencialidad del sistema, sino la creacion de secuencias segun el diseño que se desee y que pueda facilitar el manejo de multiconfiguraciones y/o la compartición de sistemas complejos donde se insertan o derivan canales o bloques de elementos ópticos.

Entre las opciones barajadas siguen pesando la incorporación de rutinas específicas de cada paquete o la creación de interfaces específicas para interaccionar con cada paquete. Los pros y contras de cada uno son variados y parece que cada interesado prefire configuraciones muy independientes. El conversor de espesores no está resultando tan obvio o fácil como esperabamos y las diferentes formas de manejar cada uno de los elementos comvierte la idea en un maremagnum de comandos y accesos a APIs que no sé si puede compensar respecto al desarrollo nuevo independiente o basandose en un unico fork.

Ha surgido este fin de semana una propuesta de apoyar el paquete Optiland-AI que podría tener visos de futuro. Voy a estudiar este caso e informarme sobre la aplicación y entrenamiento de sistemas AI para desarrollo y optimización de sistemas ópticos.

Espero dejar una primera toma de contacto con la estructura del programa antes de vacaciones y en último caso, si no se me viene el inició de un proyecto que está elaborandose en mi trabajo y que puede arrancar justo a la vuelta de vacaciones, implementar algo funcional para, al menos, crear el sistema y hacer un trazado de rayos con las definiciones que me he propuesto.
