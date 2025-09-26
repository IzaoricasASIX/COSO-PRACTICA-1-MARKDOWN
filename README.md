1 Taller de introducción a Markdown
1.1 ¿Qué es Markdown?
Markdown es un lenguaje de marcado ligero creado por John Gruber y Aaron Swartz que trata de facilitar la redacción y lectura de documentos en texto plano, utilizando un conjunto de etiquetas muy sencillas para aplicar estilo al documento.

Actualmente no existe un estándar para Markdown, por este motivo existen diferentes versiones o flavors de Markdown.

En este curso vamos a trabajar con el flavor que se utiliza en GitHub para redactar los archivos README.md de los repositorios y la documentación técnica de los proyectos.

1.2 Etiquetas básicas de Markdown
1.2.1 Encabezados
Sintaxis Markdown:

# Esto es un ecabezado h1
## Esto es un encabezado h2
### Esto es un encabezado h3
#### Esto es un encabezado h4
##### Esto es un encabezado h5
###### Esto es un encabezado h6
HTML renderizado en GitHub:



1.2.2 Negrita y cursiva
Estilo	Sintaxis	Ejemplo	Salida
Negrita	** ** o __ __	**Texto en negrita**	Texto en negrita
Cursiva	* * o _ _	*Texto en cursiva*	Texto en cursiva
1.2.3 Resaltar un comando
Sintaxis Markdown:

En esta frase estamos resaltado el comando `ls -la`.

HTML renderizado en GitHub:

En esta frase estamos resaltado el comando ls -la.

1.2.4 Bloques de código
Al inicio del bloque se puede indicar de forma opcional cuál es el tipo de contenido que contiene el bloque para resaltar las palabras reservadas cuando se renderice. Por ejemplo: bash, python, yaml, json, html, javascript, etc.

Sintaxis Markdown:

```
sudo systemctl start apache2
```
```bash
#!/bin/bash
echo "Hola mundo"
```
```python
celsius = float(input('Introduce una temperatura en grados Celsius: '))
farenheit = (1.8 * celsius) + 32
print(f'La temperatura en grados Farenheit es: {farenheit}')
```
```yaml
version: '3'

services: 
  apache:
    build: ./apache
    ports: 
      - 80:80
    volumes:
      - ./src:/var/www/html
```
HTML renderizado en GitHub:

sudo systemctl start apache2
#!/bin/bash
echo "Hola mundo"
celsius = float(input('Introduce una temperatura en grados Celsius: '))
farenheit = (1.8 * celsius) + 32
print(f'La temperatura en grados Farenheit es: {farenheit}')
version: '3'

services: 
  apache:
    build: ./apache
    ports: 
      - 80:80
    volumes:
      - ./src:/var/www/html
1.2.5 Enlaces
Sintaxis Markdown:

[Enlace a la página web del IES Celia Viñas](https://iescelia.org)

HTML renderizado en GitHub:

Enlace a la página web del IES Celia Viñas

1.2.5.1 Otra forma de gestionar enlaces
También se pueden crear enlaces con esta sintaxis:

Enlaces a la página web del [IES Celia Viñas][1] y a [GitHub][2].

[1]: https://iescelia.org
[2]: https://github.com
Esta forma de gestionar los enlaces puede ser útil cuando vamos a utilizar el mismo enlace varias veces en el documento.

1.2.6 Imágenes
Sintaxis Markdown:

![](https://iescelia.org/web/wp-content/uploads/2012/05/iescelia_1950.jpg)

HTML renderizado en GitHub:



1.2.7 Listas
1.2.7.1 Listas desordenadas
Sintaxis Markdown:

* Item 1
* Item 2
* Item 3
* Item 4
HTML renderizado en GitHub:

Item 1
Item 2
Item 3
Item 4
1.2.7.2 Listas desordenadas anidadas
Sintaxis Markdown:

* Item 1
  * Item 1.1
  * Item 1.2
* Item 2
  * Item 2.1
* Item 3
* Item 4
HTML renderizado en GitHub:

Item 1
Item 1.1
Item 1.2
Item 2
Item 2.1
Item 3
Item 4
1.2.7.3 Listas ordenadas
Sintaxis Markdown:

1. Item 1
2. Item 2
3. Item 3
4. Item 4
HTML renderizado en GitHub:

Item 1
Item 2
Item 3
Item 4
1.2.7.4 Listas ordenadas anidadas
Sintaxis Markdown:

1. Item 1  
  1.1 Item 1.1  
  1.2 Item 1.2  
2. Item 2  
  2.1 Item 2.1  
3. Item 3  
4. Item 4  
HTML renderizado en GitHub:

Item 1
1.1 Item 1.1
1.2 Item 1.2
Item 2
2.1 Item 2.1
Item 3
Item 4
1.2.8 Tablas
Sintaxis Markdown:

| Encabezado 1 | Encabezado 2 | Encabezado 3
| --- | --- | --- 
| Fila 1.1 | Fila 1.2 | Fila 1.3
| Fila 2.1 | Fila 2.2 | Fila 2.3
| Fila 3.1 | Fila 3.2 | Fila 3.3
HTML renderizado en GitHub:

Encabezado 1	Encabezado 2	Encabezado 3
Fila 1.1	Fila 1.2	Fila 1.3
Fila 2.1	Fila 2.2	Fila 2.3
Fila 3.1	Fila 3.2	Fila 3.3
1.2.9 Forzar un salto de línea
Para forzar un salto de línea es necesario incluir dos espacios en blanco y un salto de línea.

Sintaxis Markdown:

Por ejemplo, en esta frase  
hemos forzado un salto de línea.
HTML renderizado en GitHub:

Por ejemplo, en esta frase
hemos forzado un salto de línea.

1.2.10 Citar textos
Sintaxis Markdown:

Este texto no es una cita.
> Este texto daría como resultado una cita.
HTML renderizado en GitHub:



1.2.11 Comentarios
Para poner un comentario en Markdown y que su contenido no sea renderizado, se utiliza la misma sintaxis que los comentarios de HTML.

Sintaxis Markdown:

Párrafo 1.

<!- Este texto es un comentario y no será renderizado -->

Párrafo 2.
HTML renderizado en GitHub:

Párrafo 1.

Párrafo 2.




https://github.com/IzaoricasASIX/COSO-PRACTICA-1-MARKDOWN/blob/main/images/Image.jpg


<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/2263823f-135d-4d0b-b389-71397c16882d" />

