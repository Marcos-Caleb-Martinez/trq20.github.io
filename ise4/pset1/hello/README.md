# Hola mundo!
---

## Problema
---
A modo de actividad introductoria, vamos a empezar por el programa mas sencillo que es el de poder ingresar un nombre por la consola e imprimir un saludo.

## Especificaciones
---
Implementar en un archivo `hello.c` dentro de una carpeta `pset1/hello` un programa que resuelva lo planteado arriba.

El programa debe:
- Imprimir un mensaje pidiendo el nombre de la persona que ejecuta el programa.
- Imprimir un mensaje saludando a la persona que ingresó el nombre.

El programa debe comportarse de esta manera:

```
$ ./hello
Como es tu nombre? Fabrizio
Hola Fabrizio!
```

## Orientación
---

[![](https://img.youtube.com/vi/ID)](LINK A VIDEO)

- Van a necesitar trabajar con un tipo de dato especial, una cadena de caracteres, que en otros lenguajes se denomina `string`. No vamos a entrar en detalles ahora en lo que es una cadena de caracteres, pero vamos a declararla de la siguiente forma:

```c
char name[20];		   // Puedo almacenar hasta 20 caracteres 
```

- Para tratar con esta cadena, sugerimos la función `gets` para poder hacerlo de forma mas sencilla:

```c
gets(name);	// Entre parentesis pasamos la variable donde queremos guardar el texto
```

## Como probar el código
---
Compilen el programa escribiendo en la terminal:

```
gcc -o hello hello.c
```

Van a ver aparecer un `hello.exe`. Luego ejecuten el programa escribiendo:

```
./hello
```

Asegúrense de que el programa se comporte de la manera apropiada, especialmente para casos donde el que ejecute el programa tenga mas de un nombre o decida poner su nombre y apellido.

## Como entregar
---
Dentro de la carpeta `pset1/hello` abrir la terminal y escribir `git init`. Luego, crear un archivo dentro de la carpeta que se llame `README.md`. El archivo debe tener este contenido:

```markdown
# Hello

Alumno: Nombre y apellido
Curso: Curso
Materia: Control de Interfaces
```

Pueden agregar cualquier comentario u observación adicional que crean que pueda ser útil dentro de este archivo.

En la terminal ahora corran los comandos:

```
git add hello.c README.md
git commit -m "Initial commit"
git checkout -b ise4/2021/c/hello
```

Por ultimo, hacer un push de la rama que recién crearon al repositorio en GitHub con:

```
git push https://github.com/trq20/USERNAME.git ise4/2021/c/hello
```

Recuerden cambiar `USERNAME` por su nombre de usuario en GitHub. Pueden verificar si la entrega se hizo visitando el repositorio en `https://github.com/trq20/USERNAME/tree/ise4/2021/c/hello`. Si al entrar al link no encuentran nada, vuelvan a verificar los pasos de esta sección.