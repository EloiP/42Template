# 42Template
Plantilla basica para mis proyectos de 42, me ahorrara tiempo en el futuro o eso espero.

## Carpetas

La plantilla consta de entre 1 y 7 tipos de carpeta.

### Notacion

**\{E}**: Son carpetas que han de ser eliminadas antes de entregar el proyecto porque son consideradas "Innecesarias".

**\{M}**: Son carpetas generadas por el makefile y eliminadas por el mismo.

**\{N}**: Puede haber multiples carpetas de este tipo.

---

### {E}Fuentes
La carpeta [Fuentes](./Fuentes) es donde guardo un README con los links de los tutoriales y paginas que he consultado, con un subject y si encuentro la hoja de correccion tambien.

### Source code
La carpeta [source](./src) es donde guardo los .c del codigo, intento poner un .c por funcion, y quizas una subcarpeta por parte importante del proyecto.

### {E}Testers

La carpeta [testers](./testers) consta de varias carpetas, la que se llama [Eloi](./testers/Eloi) contiene los tests que yo mismo he programado o realizado. El resto de carpetas son testers que otras personas han realizado.

### {N}libn

La carpeta libn contiene una libreria con su propio makefile y carpeta Includes, puede haber muchas librerias necesarias para un proyecto, asi que puede haber muchas de estas.

### {M}Objs

La carpeta objs contiene todos los objetos generados, lo qual hace mas facil ver errores y resulta en carpetas y codigo mucho mas limpio.

### {M}libs

La carpeta libs contiene todas las librerias compiladas, lo qual hace mas facil ver cual falla y cual no.

### {M}Includes

La carpeta includes contiene todos los .h del proyecto, esto facilita su uso y hace que todo sea mas ordenado.

### .git

La carpeta .git gestiona todo lo relacionado con el proyecto de github, asi que esta bien eliminarla cuando vayas a pasarlo a la repo de 42.

## Archivos

### README.md

El readme de los proyectos de 42 lo gestiono distinto a los readme habituales, ya que no hay contribuciones de otras personas ni Badges ni Licencias ni sera Instalado ni ejecutado.

Los divido en los siguientes apartados, Hay un [archivo](ejemplo.md) con los apartados ya creados para facilitarme la gestion.

Se divide en:
- Titulo
- Descripcion
- Quehaceres
- Teoria
- Funciones
- Librerias
- Ideas abandonadas
- Libft

### Makefile

Tiene las siguientes normas:
- all: Compilacion habitual
- re: Recompila todo
- clear: Limpia objetos y librerias
- fclear: Limpia tambien ejecutables
- norm: Pasa la norminette
- bonus: Compila los bonus, si hay.
- mem: Pruebas de memoria con valgrind.
- test: Pruebas con testers propios o de otra gente.

## Uso

1- Clona el repositorio

2- Copia las carpetas de las librerias y asegurate de que tengan la estructura con carpeta de Includes

3- Modifica el makefile para el nombre del proyecto y las normas, ten presente que usa una wildcard para coger todo lo que haya dentro de la carpeta src.

4- Haz el proyecto dentro de [source](./src) y con el [header](./src/Includes)

5- Haz tus propios testers o utiliza los de otros en la carpeta tester, si quieres crea una norma test en el makefile.

6- Elimina las carpetas y archivos \{E} Ya que son tecnicamente innecesarios para la compilacion y la correccion.

7- Copia esta repo en la repo del ejercicio de 42 y pushea.
