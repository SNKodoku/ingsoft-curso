<div style="display: table;">
    <div style="width: 75%;float: left;margin: auto;padding: 50px 0px 50px 10px; float: left;">
        <span style="color: black;font-size: 25px;font-weight: bold;">UNIVERSIDAD NACIONAL AUTÓNOMA DE MÉXICO</span></br></br>
        <span style="color: black;font-size: 26px;">FACULTAD DE ESTUDIOS SUPERIORES ACATLÁN</span>
    </div>
    <img src="/archivos/index/fesa.png" alt="drawing" width="200" style="width: 25%;"/>
</div>

# ¿Qué es JSON y XML?

## JSON
Sus siglas en ingles son por JavaScrispt Object Notation. Es un formato que guarda e intercambia información que se pueda leer y entender por cualquier usuario, y esta principalmente se usa para transferir datos entre el servidor y cualquier cliente.

Los archivos json almacenan únicamente texto y estas mismas usan la extensión .json; el archivo es una alternativa más común y menos pesada al XML (Lenguaje de marcado extenso) que cuanta con funciones similares.

Los desarrolladores usan Json para trabajar con AJAX (JavaScript asíncrono y XML) donde estos formatos funcionan en sintonía juntos para conseguir la carga asincrónica de los datos almacenados.

JSON se basa en dos estructuras:

Un objeto es un conjunto desordenado de pares de nombre / valor. Un objeto comienza con {llave izquierda y termina con} llave derecha. Cada nombre va seguido de: dos puntos y los pares de nombre / valor están separados por una coma.

## CARACTERISTICAS
JSON es un lenguaje de modelador de datos
* Consiste en pares "clave - valor"
* Los valores pueden cadenas, números o boléanos, así como otros objetos JSON, con cualquier nivel de anidación
* Es un formato flexible, ligero y fácilmente transferible a través de las redes
* En JSON, adoptan estas formas:

Un objeto es un conjunto desordenado de pares de nombre / valor. Un objeto comienza con {llave izquierda y termina con} llave derecha. Cada nombre va seguido de: dos puntos y los pares de nombre / valor están separados por una coma.
<img src="/archivos/index/JSON.png">

Una matriz es una colección ordenada de valores. Una matriz comienza con [corchete izquierdo y termina con] corchete derecho. Los valores están separados por coma.
<img src="/archivos/index/array.png">

Un valor puede ser una cadena entre comillas dobles, un número, verdadero, falso, nulo, un objeto o una matriz. Estas estructuras se pueden anidar.
<img src="/archivos/index/value.png">

Una cadena es una secuencia de cero o más caracteres Unicode, entre comillas dobles, utilizando escapes de barra invertida. Un carácter se representa como una sola cadena de caracteres. Una cadena es muy parecida a una cadena C o Java.
<img src="/archivos/index/number.png">

Se pueden insertar espacios en blanco entre cualquier par de tokens. Excepto algunos detalles de codificación, eso describe completamente el idioma.
<img src="/archivos/index/whitespace.png">

## VENTAJAS Y DESVENTAJAS DE JSON.

 |                                VENTAJAS                                  |	                             DESVENTAJAS                                   |
 |--------------------------------------------------------------------------|------------------------------------------------------------------------------|
 | Es auto descriptivo y fácil de entender.                                  | Algunos desarrolladores encuentran su escueta notación algo confusa.         |
 | Su sencillez le ha permitido posicionarse como alternativa a XML.        | No cuenta con una característica que posee XML: extensibilidad.              |
 | Es más rápido en cualquier navegador.                                    | No soporta grandes cargas, solo datos comunes.                               |
 | Es más ligero (bytes) en las transmisiones.                              | Para la seguridad requiere de mecanismos externos como expresiones regulares.|
 | Velocidad de procesamiento alta.                                         |                                                                              |
 | Puede ser entendido de forma nativa por los analizadores de JavaScript.  |                                                                              |
 | Es más fácil de leer que XML.                                            |                                                                              |
 | Se parase más rápido.                                                    |                                                                              |

## EJEMPLOS
 Ejemplo de objeto JSON en JavaScript

var misDatosJson = {"menu": {
  "id": "archivo",
  "valor": "Archivo",
  "popup": {
    "menuitem": [
      {"value": "Nuevo", "onclick": "CrearNuevoDocumento()"},
      {"value": "Abrir", "onclick": "AbrirDocumento()"},
      {"value": "Cerrar", "onclick": "CerrarDocumento()"}
    ]
  }
}}

Ejemplo de acción que devuelve una cabecera JSON

class publicacionesActions extends sfActions
{
  public function executeActualizar()
  {
    $resultado = '[["titulo", "Mi carta normal"], ["nombre", "Sr. Pérez"]]';
    $this->getResponse()->setHttpHeader("X-JSON", '('.$resultado.')');

    return sfView::HEADER_ONLY;
  }
  
  Ejemplo de lista ordenable

<p>What do you like most?</p>
<ul id="ordenar">
  <li id="elemento_1" class="ordenable">Zanahorias</li>
  <li id="elemento_2" class="ordenable">Manzanas</li>
  <li id="elemento_3" class="ordenable">Naranjas</li>
  // A nadie le gustan las coles de Bruselas
  <li id="elemento_4">Coles de Bruselas</li>
</ul>
<div id="respuesta"></div>
<?php echo sortable_element('ordenar', array(
  'url'    => 'elemento/ordenar',
  'update' => 'respuesta',
  'only'   => 'ordenable',
)) ?>
 
## XML
Se trata de un lenguaje de marcado el cual se encarga de definir un conjunto de reglas que estas permiten codificar documentos.

Un archivo XML está dividido en dos partes:
* Prolog
Esta consiste en metadatos administrativos, como declaración XML, instrucción de procesamiento opcional, declaración de tipo de documento y comentarios.

* Body
Esta parte se compone de dos partes: estructural y de contenido (presente en los textos simples).
 
Un documento XML está formado por datos de caracteres y marcado, el marcado lo forman las etiquetas:
<img src="/archivos/index/formato xml.png">

Su estructura está compuesta por:
<img src="/archivos/index/formato.png">

## CARACTERISTICAS.
* XML es un subconjunto de SGML que incorpora las tres características más importantes de este:
 * Extensibilidad
 * Estructura
 * Validación
* Basado en texto.
* Orientado a los contenidos no presentación.
* Las etiquetas se definen para crear los documentos, no tienen un significado preestablecido.
* No es sustituto de HTML.
* No existe un visor genérico de XML.

## VENTAJAS Y DESVENTAJAS DE XML.

 |                                VENTAJAS                                                                |	                             DESVENTAJAS                                               |
 |--------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------|
 | Tiene un formato estructurado y fácil de comprender.                                                   | El formato es sumamente estricto.                                                      |
 | Separa radicalmente la información o el contenido de su presentación o formato.                        | Lleva más tiempo procesarlo.                                                           |
 | Está diseñado para ser utilizado en cualquier lenguaje o alfabeto.                                     | Complejidad de analizador (parser).                                                    |
 | Su análisis sintáctico es fácil debido a las estrictas reglas que rigen la composición de un documento.| Un error en cualquier parte del formato puede hacer que todo el documento sea inválido.|
 | Tiene soporte a cualquier tipo de datos.                                                               |                                                                                        |
 | Se pueden definir estructuras complejas y reutilizables.                                               |                                                                                        |
 
Los archivos JSON 
Contenido:
Definir qué es JSON
Definir qué es XML
Indicar características
Indicar usos
Indicar Ventajas y Desventajas
Agregar una tabla comparativa
Agregar al menos 3 ejemplos (Cada ejemplo debe estar representado tanto en XML y JSON respectivamente).

## EJEMPLOS
Ejemplo de Estructura XML
<?xml version=" 1.0 " encoding=" UTF-8 " standalone= " yes "?>
<ficha>
<nombre> Gabriel </nombre>
<apellido> Molina </apellido>
<direccion> Alfredo Vargas #36 </direccion>
</ficha>

Ejemplo de Menú De Comidas En XML
<menu_almuerzo>
    <comida>
        <nombre>Waffles</nombre>
       <precio>$2.00</precio>
        <descripcion>Waffles baratos de McDonalds</descripcion>
        <calorias>650</calorias>
    </comida>
    <comida>
        <nombre>Hamburguesa</nombre>
        <precio>$5.00</precio>
        <descripcion>La hamburguesa mas comun de McDonalds</descripcion>
        <calorias>1500</calorias>
    </comida>   
</menu_almuerzo>

Ejemplo de Catálogo De CDs En XML
<CATALOGO>
    <CD>
        <TITULO>Tinta roja</TITULO>
        <ARTISTA>Andres Calamaro</ARTISTA>
        <ORIGEN>AR</ORIGEN>
        <PRECIO>5.90</PRECIO>
        <ANO>2006</ANO>
    </CD>
    <CD>
        <TITULO>La Lengua Popular</TITULO>
        <ARTISTA>Andres Calamaro</ARTISTA>
        <ORIGEN>AR</ORIGEN>
        <PRECIO>9.90</PRECIO>
        <ANO>2007</ANO>
    </CD>
</CATALOGO>

## REFERENCIAS
https://www.ejemplode.com/21-xml/35-ejemplo_de_estructura_xml.html#ixzz78di6buHz
https://www.json.org/json-en.html
https://desarrolloweb.com/home/json
