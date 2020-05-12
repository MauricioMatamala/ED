# Recuperación del segundo trimestre

Se realizará una prueba el próximo martes 19.

| Tipo de Examen | Fecha y Hora | Detalles |
|------|----------------|--------------|
| Examen presencial | 19/5/2020 16:00 - 20:00 | Reunión por Google Meeting enviada por correo |

# Procedimiento del examen

Se  propondrán ejercicios de los siguientes temas:

- UML
- Maven

Cualquier duda que surja la podemos aclarar en la reunión de Google Meeting correspondiente al examen, en la que el profesor estará conectado todo el tiempo.

# Actividades de repaso para la Recuperación del segundo trimestre.

Para que podáis preparar el examen os propongo algunas cosas que podéis hacer:

- UML
    - Revisar la documentación de la página [http://www.politecnico-ed.es/ED/uml.html](http://www.politecnico-ed.es/ED/uml.html).
    - Intentar hacer los ejercicios propuestos en dicha página.
- Maven
    - Revisar la documentación de la página [http://www.politecnico-ed.es/ED/maven.html](http://www.politecnico-ed.es/ED/maven.html) hasta el apartado **Servidor Nexus* (no es necesario que practiquéis este apartado -ver nota más abajo-).
    - Intentar hacer los siguientes ejercicios (esencia de lo que se pedirá en el examen sobre *Maven*).

> NOTA: El servidor Nexus no entra dentro de lo que se podría considerar un exámen de mínimos. Por ello, y debido a los potenciales problemas durante el examen relacionados con el servidor (y no con Maven) no entrará en el examen.

**Actividad de repaso 1.** Crea un nuevo proyecto, llamado Aritmetica que incluye una clase llamada **Multiplicacion**. Después genera un archivo .jar. Finalmente instala el archivo .jar en el repositorio local de *Maven*..

Una vez hecho esto, crea un nuevo proyecto llamado **TablaMultiplicar** que tenga como dependencia al proyecto **Aritmetica**. Incluye el proyecto en el *POM*, y muestra por pantalla la tabla de multiplicar de un número utilizando la clase Multiplicacion.

**Actividad de repaso 2.** Repite el ejercicio anterior, pero en este caso sube el proyecto **Aritmetica** a *GitHub*. Después, añade la dependencia al proyecto **TablaMultiplicar**, y muestra por pantalla la tabla de multiplicar de un número utilizando la clase Multiplicacion.
