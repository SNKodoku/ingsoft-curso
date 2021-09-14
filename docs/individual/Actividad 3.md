# Ingeniería de Requerimientos
## ¿Qué es UML?
El UML fue creado para contruir un lenguake de modelado visual comun y semantica y sintacticamente rico para la arquitectura, el diseño y la implementacion de sistemas de software complejos tanto en estructuracomo en comportamiento. 

Es un lenguaje de modelado visual de proposito general orientado a objetos y comparable a los planos usados en otros campos y consiste en diferentes tipos de siagramas. EN general, los diagramas UML secriben los limites, la estructura y el comportamiento del sistema y los objetos que contiene.

Cubre toda la documentacion de un sistema:
* Aquitectura del sistema u sus detalles.
* Expresar requisitos y pruebas.
* Modelar las actividades de planificacion y gestion de versiones.
## Caracteristicas
Ofrece vocabulario y reglas:
* Para crear y leer modelos bien formados
* Que constituyen los planos de un sistema de software.

Es independiente del proceso de desarrollo
* Un uso optimo se consigue en procesos dirigdos por casos de uso, centrados en la arquitectura, iterativos e incrementales.

Cubre la diferentes vistas de la arquitectura de un sistema mientras evoluciona a traves del ciclo de visa del desarrollo de software.

## Ventajas
Ventajas de UML
* Es estándar => Facilita la comunicación
* Está basado en metamodelo con una semántica bien definida
* Se basa en una notación gráfica concisa y fácil de aprender y utilizar
* Se puede utilizar para modelar sistemas software en diversos dominios:
* Sistemas de información empresariales, Sistemas WEB, sistemas críticos y de tiempo real, etc.
* Incluso en sistemas que no son software
* Es fácilmente extensible

## Ejemplo

![Mi Imágen](/docs/individual/Actividad-02/ejemplo uml.png) 

## ¿Que es un Diagrama?
Es un dibujo geometrico con el que se genera la presentacion grafica de una proposicion, de la resolucion de un problema, de las relaciones entre las diferentes partes o elementos de un conjunto o sistema, o de la regularidad en la variacion de un fenomeno que permite establecer algun tipo de ley.

## Diagrama de objetos
"Un diagrama de objetos es un gráfico de instancias, incluyendo objetos y datos. Un diagrama de objetos es una instancia de un diagrama de clases; muestra una 'foto' del estado de un sistema en un punto de tiempo determinado." 
                                                Object Management Group.

Algunos elementos de los diagramas de objetos son:

Objetos: Cada objeto se representa con un rectángulo con su nombre y el de su clase en la parte superior subrayados y separados por dos puntos. En caso de ser un objeto anónimo no se escribe su nombre, dejando solo el de la clase.

Atributos: De igual forma que el diagrama de clases, se muestra en un compartimento en la parte inferior del nombre del objeto. A diferencia de las clases, los atributos pueden tener valores asignados a ellos

Vínculos: Son asociaciones entre dos objetos y se representan con los mismos elementos que en el diagrama de clases. Por ejemplo, una asociación:

## Diagrama de Paquetes
El diagrama de paquetes muestra como un sistema esta dividido en agrupaciones logicas mostrando las dependencias entre esas agrupaciones. En un paquete normalmente esta pensado como un directorio, los diagramas de paquetes suministran una descomposicion de la jerarquia logica de un sistema y maximiza la coherencia enterrna dentro de cada paquete y minimiza el acoplamiento extremo entre los paquetees.

Estas mismas representan dependencias entre los paquetes que componen un modelo, muestra como un sistema esta dividido en agrupaciones logicas y las dependencias entre agrupaciones

Las dependencias entre paquetes denotan que algún elemento de un paquete depende de los elementos en otro paquete. Existen diferentes tipos de relaciones de dependencia entre paquetes:

Importación: Modelado como una dependencia estereotipada con <<import>>.
Acceso: Modelado como una dependencia estereotipada con <<access>>.
Combinación: Modelado como una dependencia estereotipada con <<merge>>.
Exportación: Modelado implícitamente a través de la visibilidad pública en los elementos del paquete. No se exporta explícitamente a algún paquete.

## Diagrama de Tiempos
Es una grafica de ondas digitale, esta muestra la realacion temporal entros algunas señales, y como varia cada señal en relacion a las demas. Estas representan en una linea temporal los cambios que se producen en uno o varios objetos, respondiendo a los eventos que se producen en el sistema de informacion.

Algunos de sus elementos son:

Línea de vida
La línea de vida es un elemento que representa a un participante individual en la interacción

Estado
El diagrama de tiempo podría mostrar los estados del clasificador o atributo participante, o algunas condiciones comprobables, como un valor discreto de un atributo.

Restricción de duración
La restricción de duración es una restricción de intervalo que se refiere a un intervalo de duración. El intervalo de duración es la duración que se utiliza para determinar si se cumple la restricción.

Restricción de tiempo
La restricción de tiempo es una restricción de intervalo que se refiere a un intervalo de tiempo. El intervalo de tiempo es una expresión  utilizada para determinar si se cumple la restricción.