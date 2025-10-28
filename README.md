# AHF Documentacion BOM (Browser Object Model)
| DWEC JAVASCRIPT BOM |
|:-----------:|
![Alt](images/banner%20javascript.jpg)|
| DESARROLLO WEB ENTORNO CLIENTE |



## 1. BOM JAVASCRIPT (Browser Object Model)

Este documento es una documentación sobre el BOM de Javascript , conteniendo en ella toda la información necesaria asi como los métodos o los objetos que lo componen.

### 1.1 ¿Que es el BOM? (Browser Object Model)

El BOM (Browser Object Model o Modelo de Objetos del Navegador) es un conjunto de objetos y propiedades que permite a JavaScript interactuar con el navegador y su entorno, controlando elementos como la ventana, el historial o las alertas. A diferencia del DOM (Modelo de Objetos del Documento), que se enfoca en el contenido HTML de una página, el BOM maneja el entorno del navegador en sí.



### 1.2 Componentes principales del BOM 

![Alt](images/estructura%20BOM.webp)

En esta imagen podemos comprobar la estructura de árbol que tiene el BOM , desde el elemento raiz Window hasta todos sus hijos como el Document el cual representa el DOM (Document Object Model).

  #### Window: 

  Es el objeto raíz y el punto de entrada al BOM. Representa la ventana del navegador y contiene todos los demás objetos. (Es soportado por todos los navegadores).
  - MÉTODOS: 

    - window.open() : Abre una nueva ventana.
    - window.close() : Cierra la ventana actual.
    - window.moveTo() : Mueve la ventana actual.
    - window.resizeTo() : Redimensiona la ventana.
    - alert() : Muestra una alerta en la ventana.


  #### Document Object

  El objeto Document es hijo de Window y representa la parte del DOM (Document Object Model) , con todos sus métodos y nodos en conjunto.

  Representa el nodo root de un documento HTML.

  Se puede acceder a el mediante window.document() o simplemente document().

![Alt](images/estructuraDOM.png)


 - MÉTODOS: 
  
    Los siguientes métodos y propiedades pueden ser usados en los documentos HTML.

    - activeElement() : Devuelve el elemento con el foco del documento.
    - getElementByid() : Devuelve el elemento del documento HTML con dicha id.
    - write() : Escribe expresiones HTML o JavaScript en el documento.
    - URL : Devuelve la url completa del documento.

#### History Object 

El objeto History contiene las urls que han sido visitadas por el usuario (En la ventana del navegador).

Es una propiedad del objeto Window.

Se puede acceder a el mediante: 

```bash
window.history()
```

```bash
history()
```

- MÉTODOS Y PROPIEDADES: 

    - back() : Carga la url anterior de la lista del historial.
    - forward() : Cargar la siguiente url en la lista del historial.
    - go() : Cargar una url en especifico de la lista del historial.
    - length() : Devuelve el numero de url en el historial.


#### Screen Object 

El objeto Screen contiene información sobre la pantalla o el monitor del cliente.

- PROPIEDADES DEL OBJETO SCREEN:

    - availHeight : Devuelve la altura de la pantalla.
    - availWidth : Devuelve la anchura de la pantalla.
    - colorDepth : Devuelve la cantidad de bits de la paleta de colores.
    - height: Devuelve la altura total de la pantalla.
    - pixelDepth : Devuelve la resolución de color (bits por pixel).
    - width: Devuelve la anchura total de la pantalla.


#### Location Object 

El objeto Location contiene información sobre la URL actual.

Se puede acceder a el mediante 

```bash
window.location 
```

O simplemente: 

```bash
location 
```

 - PROPIEDADES DEL OBJETO LOCATION: 

    - host : Devuelve el hostname y el numero de puerto de la URL.
    - href : Devuelve la URL entera.
    - pathname : Devuelve el nombre del path de la URL.
    - port: Devuelve el numero de puerto.
    - protocol : Devuelve el protocolo.


 - MÉTODOS DEL OBJETO LOCATION:

    - assign() : Carga un nuevo documento.
    - reload() :  Recarga el documento actual. 
    - replace() : Sustituye el documento por otro nuevo.



#### Console Object 

El objeto Object proviene de acceso a la consola de debug del navegador.

Es una propiedad del objeto Window.

Se puede acceder a el mediante: 

```bash
window.console
```

O simplemente: 

```bash
console
```

 - MÉTODOS DEL OBJETO CONSOLE: 
    - assert() : Escribe un mensaje de error en la consola si la aserción es falsa.
    - clear() : Limpia la consola.
    - error () : Salida de un mensaje de error por consola.
    - log() : Salida de un mensaje por consola (Sea cual sea el mensaje).
    - warn() : Salida de un mensaje de warning por consola.

Alejandro De la Huerga Fernández (28-10-2025)

