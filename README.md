# Actividad 2 - markdown
> Autor: Óscar Regalado León.  
>Fecha: Mayo 2026.
---
## 1. Lista ordenada.
Para realizar una lista ordenada, simplemente aplicamos el números precedidos de . como se muestra en el siguiente ejemplo.

~~~
Esto es la inserción de una lista ordenada en markdown:
1. Elemento 1
2. Elemento 2
~~~

Como resultado obtendríamos:

Esto es la inserción de una lista ordenada en markdown:
1. Elemento 1
2. Elemento 2

## 2. Lista desordenada.
Para una lista desordenada se sigue el mismo patrón pero en vez de números usamos los símbolos {*,+,-}.

~~~
Esto es la inserción de una lista desordenada en markdown:
* Elemento 1
* Elemento 2
~~~

Como resultado obtendríamos:

Esto es la inserción de una lista desordenada en markdown:
* Elemento 1
* Elemento 2

## 3. Tabla.
Para la elaboración de la tabla seguimos el siguiente patrón de inserción:

~~~
| columna 1 | columna 2 | columna 3 |
| --------- | --------- | --------- |  <!-- línea de separación -->
| valor f1,C1 | valor f1,C2 | valor f1,c3 |
| valor fn,C1 | valor fn,C2 | valor fn,c3 |
~~~
Como resultado obtendríamos:
| columna 1 | columna 2 | columna 3 |
| --------- | --------- | --------- |   
| valor f1,C1 | valor f1,C2 | valor f1,c3 |
| valor fn,C1 | valor fn,C2 | valor fn,c3 |  

## 4. Imágenes insertadas.

Las imágenes se pueden insertar dos modos:

### 4.1 Con acceso local.

Para insertar una imagen con acceso local utilizamos la siguiente sintaxis:

~~~
![título imagen](ruta de la imagen)
~~~
Si colocamos la imagen en el mismo directorio que el documento **.md** simplemente en la ruta debemos especificar en nombre de la imagen.formato.

Ejemplo:

~~~
![esquema BBDD](MR_Ejercicio_1_BBDD.drawio.svg)
~~~
Se visualiza:
![esquema BBDD](MR_Ejercicio_1_BBDD.drawio.svg)

### 4.2 Con acceso externo.

Para insertar una imagen con acceso externo empleamos la siguiente sintaxis:

~~~
![título imagen](URL de la imagen)
~~~

Ejemplo:

~~~
![esquema BBDD](https://hd.wallpaperswide.com/thumbs/windows_xp_original-t2.jpg)
~~~

Se visualiza:

![esquema BBDD](https://hd.wallpaperswide.com/thumbs/windows_xp_original-t2.jpg)

## 5. Accesos a páginas web.

Para generar un link, aplicamos la siguiente sintaxis:

~~~
[Texto resaltado](URL)
~~~

Por ejemplo:

~~~
[Xataka](https://www.xataka.com/)
~~~

Se visualizaría así:

[Xataka](https://www.xataka.com/)

## 6. Cita.

En este documento hemos generado ya un ejemplo de cita, en el encabezado, el autor y fecha están realizados con cita, para ello aplicamos el símbolo \> y luego un espacio y texto.

~~~
> Esto es una cita.
~~~

Se visualiza así:

> Esto es una cita.


## 7. Secciónes de código.

Por último, como hemos realizado a lo largo del documento, vemos la sintaxis para realizar blóques de código para dos lenguajes de programación distintos:

### 7.1. Lenguaje de programación Python:

Escribimos el código haciendo referencia, inmediatamente después del primer ~~~ o ''' del lenguaje de programación python. Debemos cerrar la sección con nuevamente \~~~ o \'''.

~~~python
# variables
try:
    a = int(input("Introduce el valor de a: "))
    b = int(input("Introduce el valor de b: "))
except ValueError:
    print("Introduce un valor entero.")
# Programa
if a < b:
    print(f"El número {a} es menor a {b}.")
else:
    print(f"El número {b} es menor a {a}.")
~~~

### 7.2. Lenguaje de marca extensible xml:

Procedemos de igual manera que en el apartado anterior, pero especificando la palabra xml.

~~~xml
<?xml version="1.0" encoding="UTF-8"?>
<note>
  <to>Tove</to>
  <from>Jani</from>
  <heading>Reminder</heading>
  <body>Don't forget me this weekend!</body>
</note>
~~~