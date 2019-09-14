## [Introducción a la interfaz](https://www.jetbrains.com/help/idea/guided-tour-around-the-user-interface.html)
![Descripción de las partes de la interfaz](https://www.jetbrains.com/help/img/idea/2019.2/ij_mainWindow_default.png)
### [Editor](https://www.jetbrains.com/help/idea/using-code-editor.html)
- Archivos abiertos (en la parte de arriba)
- Hilo de ariadna (en la parte inferior indicando la ubicación en la clase)
- Números de línea a la izquierda
- Barra de scroll

#### [Cambiar la apariencia del editor](https://www.jetbrains.com/help/idea/using-code-editor.html#04696ee6)
Settings -> Editor -> Color Scheme

#### [Cambiar la configuración de las pestañas](https://www.jetbrains.com/help/idea/using-code-editor.html#manage_tabs)
Settings -> Editor -> General -> Editor Tabs

#### [Dividir la pantalla del editor](https://www.jetbrains.com/help/idea/using-code-editor.html#split_screen)
Clic sobre la pestaña del editor

#### [Configuraciones útiles del editor](https://www.jetbrains.com/help/idea/using-code-editor.html#editor_settings)


### [Status bar](https://www.jetbrains.com/help/idea/guided-tour-around-the-user-interface.html#status-bar)

### [Tool window](https://www.jetbrains.com/help/idea/guided-tour-around-the-user-interface.html#tool-windows)
Ofrecen funcionalidad adicional, como mostrar el árbol del proyecto, o mostrar el resultado de una ejecución.

### [Temas de usuario](https://www.jetbrains.com/help/idea/user-interface-themes.html#User_interface_themes.xml)
Se pueden cambiar en *Settings ->  Appearance & Behavior -> Appearance*

### [Modos de visualización](https://www.jetbrains.com/help/idea/ide-viewing-modes.html#IDE_Viewing_Modes.xml) 
Menú *View -> Appearance*
 - Full Screen
 - Distraction-free
 - Presentation

### [Atajos de teclado](https://www.jetbrains.com/help/idea/mastering-keyboard-shortcuts.html)
Algunos ejemplos útiles:

- Ctrl + Shift + F10 - Run
- Ctrl + Shift + F12 - Esconder ventana de herramientas
- Ctrl + Shift + Up - mover la línea hacia arriba (Se puede hacer con selecciones)
- Ctrl + Shift + Down - mover la línea hacia abajo
- Ctrl + D - Duplicar línea
- Ctrl + Y - Borrar línea
- Shift+Shift - Buscar en todas partes
- Ctrl+Shift+A - Buscar acción
- Ctrl + N - Encontrar una clase, archivo o símbolo
- Ctrl + E - ver archivos recientes 
- Alt + Enter - sugerencias de mejora del código
- Ctrl + Space - Compleción de código
Etc.

### [Configurar los atajos de teclado](https://www.jetbrains.com/help/idea/configuring-keyboard-and-mouse-shortcuts.html#Configuring_Keyboard_and_Mouse_Shortcuts.xml)
Los atajos de teclado se pueden encontrar en *File -> Settings -> Keymap*

## [Customización de menús](https://www.jetbrains.com/help/idea/customize-actions-menus-and-toolbars.html)	

*File -> Settings -> Appearance & Behavior -> Menus and toolbars*

El símbolo "+" permite añadir una acción predefinida o un separador.
Se pueden asignar iconos a las acciones.

### [Quick lists](https://www.jetbrains.com/help/idea/customize-actions-menus-and-toolbars.html#configure_quick_lists)
Seguimos dos pasos:

 - **Crear una quick list nueva**
 	*File -> Settings -> Appearance and Behaviour -> Quick Lists*
	Se puede añadir una nueva lista, además de acciones.

 - ** Asignar un atajo de teclado a dicha quick list**
	 Añadir un nuevo  shortcut para la lista. Al hacer clic se ofrecen las opciones del menú rápido.
	*File -> Settings -> keymap -> Quicklist -> Sobre la lista (btnDer)*

 
## [Basic completion]( https://www.jetbrains.com/help/idea/auto-completing-code.html#basic_completion)
*Ctrl+Espacio* muestra las opciones que coincidan por el nombre (no decide si el tipo es adecuado o no).

	int ba = 3;
	int bo = true; 
	if ( b-> mostraría ba y bo
 
### [Autocompletado inteligente](https://www.jetbrains.com/help/idea/auto-completing-code.html#smart_completion)
*Ctrl+Shift+Espacio* muestra opciones con tipos aplicables al contexto.

	int ba = 3;
	int bo = true;
	if ( b-> completaría a bo

 
### [Autocompletado de sentencias](https://www.jetbrains.com/help/idea/auto-completing-code.html#statements_completion)

Ctrl+Shift+Enter autocompleta:
- Declaraciones de métodos
- Líneas de código
- Elige métodos de una clase
 
### [Autocompletado con sufijos](https://www.jetbrains.com/help/idea/auto-completing-code.html#postfix_completion)
 
 Opciones en File -> Settings -> Editor -> General -> Postfix completion
 
Probar: 
``` 
boolean b = true;
b.if + Tab
```
[Plugin para definir más sufijos](https://www.vojtechruzicka.com/intellij-idea-tips-tricks-postfix-code-completion/)

### [Generación de código](https://www.jetbrains.com/help/idea/generating-code.html#Generating_Code.xml)

#### Generación de código de clase
Dentro de la clase, clic derecho -> Generate o bien Ctrl+Insert:

 - Constructor
 - toString
 - Override
 - Test
 - Copyright

#### Getters/Setters
Si la clase cuenta con un campo, aparecen opciones de getters/setters al hacer clic derecho -> Generate o bien Ctrl+Insert

### [Live templates == code snippets](https://www.jetbrains.com/help/idea/using-live-templates.html#Using_Live_Templates.xml)

 - Plantillas simples: *psfs*, *psvm*, etc
 - Plantillas parametrizadas: *fori*, *ifn*

### [Configurar live templates](https://www.jetbrains.com/help/idea/using-live-templates.html#Using_Live_Templates.xml)

Abrir Settings -> Editor -> Live templates. Se pueden definir:
 - Nuevos grupos de plantillas
 - Nuevas plantillas: ¡Ojo! Al definir una plantilla hay que indicar el contexto. Ej. de plantilla:

```
	// Abbreviation -> sww
	// Al escribir *sww* + TAB
	// Cada nuevo TAB lleva a la siguiente variable
	switch ($IN$){
		case $VAL1$: $ACTION1$;
		default:	 $ACTIONN$;
	}
```

## [Navegación](https://www.jetbrains.com/help/idea/discover-intellij-idea.html#Navigation)

*Ctrl+E* -> Archivos recientes
*Ctrl+N* -> Clases disponibles
*Ctrl+Shift+N* -> Navegar archivos ( con / al final nos referimos a archivos)
*Ctrl+Shift+Alt+N* -> Navegar a un símbolo
*Alt+7* -> Estructura de una clase. En la ventana de estructura, escribiendo algo, comienza una búsqueda.

##[Refactorización](https://www.jetbrains.com/help/idea/discover-intellij-idea.html#RefactoringBasics)

Veremos sólo algunas refactorizaciones (inicialmente) en [Refactorizando el código](https://www.jetbrains.com/help/idea/refactoring-source-code.html)
Refactorizar código: Control+Shift+Alt+T

### Extract variable
```
return !b;
```
```
boolean noB = !b;
return noB;
```
### Extract field (o atributo)
Ej. Convertir *Integer.SIZE* en un atributo
```
System.out.println(Integer.SIZE); 
```

```
private static int size;
public static void main(String[] args){
	...
	System.out.println(size);
}
```
### Extract constant
```
System.out.println(3);
```
```
public static final int A=3;
.....
System.out.println(A);
```
### Extract parameter
Antes:
```
public class HelloWorldPrinter {
    public static void print() {
        System.out.println(generateText());
    }
    private static String generateText() {
        return "Hello, World!".toUpperCase();
    }
}
```
Después
```
public class HelloWorldPrinter {
    public static void print() {
        System.out.println(generateText("Hello, World!"));
    }
    private static String generateText(String text) {
        return text.toUpperCase();
    }
}
```
### Inline
Reemplaza variables redundantes. Ej.
Antes:
```
public void method() {
    int number = anotherClass.intValue();
    int b = a + number;
}
```
Después:
```
public void method() {
    int b = a + anotherClass.intValue();
}
```

### [Find usages](https://www.jetbrains.com/help/idea/discover-intellij-idea.html#FindingUsages)
Sirve para encontrar dónde se usa una variable. 

>La documentación dice que se activa con Alt+F7. En Linux no funciona este shortcut (tras buscar "Find usages" en búsqueda general con Ctrl+A), aparece como *Alt+Shift+7*.



 Sobre la variable a buscar, pulsar *Alt+Shift+7*

### [Inspections](https://www.jetbrains.com/help/idea/discover-intellij-idea.html#Inspections)

Detección de código anómalo.
*Niveles de severidad (severity level)*: Hasta donde alcanzar el problema. [Los colores](https://www.jetbrains.com/help/idea/configuring-inspection-severities.html#Configuring_Inspection_Severities.xml) permiten distinguirlos.

Un icono en la parte superior del editor muestra el estado de la inspección.
En la barra de scroll se muestran los problemas mediante líneas de color. 
	- Puntero sobre ellas, muestran problema
	- Clic sobre ellas, muestran el error y ofrecen soluciones (bombilla).
	- Dado un problema (bombilla roja) -> *Alt+Intro* ofrece soluciones	
	```
	Ej. Una clase que llama a un método inexistente en otra clase -> *Error -> Alt+Intro -> Create method...*
	```
## Annotations
Ofrecen metainformación sobre  el código. El IDE las usa para inspeccionar condiciones complejas del código. IntelliJ incluye algunas anotaciones por defecto. [Se pueden añadir más](https://www.jetbrains.com/help/idea/annotating-source-code.html#add-in-editor).

### [@NotNull y @Nullable](https://www.jetbrains.com/help/idea/nullable-and-notnull-annotations.html)
Ej. El siguiente código da error de compilación:
```
package net.mauriciomatamala;

import org.jetbrains.annotations.NotNull;

public class Anotaciones {

	public static void main(String[] args) {
		Anotaciones2 an2 = new Anotaciones2();
		an2.saludar(null);
	}
}
```
```
package net.mauriciomatamala;

import org.jetbrains.annotations.NotNull;

public class Anotaciones2 {

	public void saludar(@NotNull String saludo){
		System.out.println(saludo);
	}
}
```

*@Nullable* indica que algo puede ser null. Puede ayudar en algunos casos. Por ejemplo, un método padre *@NotNull* requiere métodos hijos *@NotNull*. En el ejemplo siguiente IntelliJ sugiere que *metodo1* debe ser @NotNull en Anotaciones2Hija.
```
package net.mauriciomatamala;

import org.jetbrains.annotations.NotNull;
import org.jetbrains.annotations.Nullable;

public class Anotaciones2 {

	@NotNull
	public Object metodo1(Object o){
		return o;
	}
}

```
```
package net.mauriciomatamala;

import org.jetbrains.annotations.NotNull;
import org.jetbrains.annotations.Nullable;

public class Anotaciones2Hija extends Anotaciones2 {

	@Override
	public Object metodo1(Object o){
		o.toString();
		return o;
	}
}
```
### [@Contract](https://www.jetbrains.com/help/idea/contract-annotations.html#@Contract_Annotations.xml)
Define la relación entre argumentos y valor devuelto. Un ejemplo (absurdo):
```
	@Contract("null -> null")
	public Boolean metodo1(Boolean b){
		return true;
	}
```
IntelliJ informa de que se viola la cláusula.

### [Anotar automáticamente @NotNull y @Nullable](https://www.jetbrains.com/help/idea/inferring-nullity.html#Inferring_Nullity.xml)
Se crean automáticamente las anotaciones en la opción *Analyze | Infer Nullity*

## [Documentación del código](https://www.jetbrains.com/help/idea/working-with-code-documentation.html#Working_with_code_documentation.xml)

Javadoc es una utilidad de Oracle para la generación de documentación de APIs en formato HTML a partir de código fuente Java. Javadoc es el estándar para documentar clases de Java. La mayoría de los IDEs utilizan javadoc para generar de forma automática documentación de clases.

La documentación que se puede aportar para una clase puede ser:

- Nombre de la clase
- Descripción general
- Número de versión
- Nombre de autores.

Documentación de cada constructor o método incluyendo información como:

- nombre del constructor o método
- tipo de retorno
- nombres y tipos de parámetros si los hay
- descripción general
- descripción de parámetros

La documentación para Javadoc ha de incluirse entre símbolos de comentario que han de empezar con una barra y doble asterisco, y terminar con un asterisco y barra simple, como por ejemplo:
```
// ARCHIVO saludo.java

package net.mauriciomatamala;

/**
 *
 * Esta clase muestra un saludo
 *
 * @author Mauricio Matamala Peinado
 * @version 0.0
 * @see <a href="http://www.mauriciomatamala.net">www.mauriciomatamala.net</a>
 *
 */
public class Saludo {

	/**
	 *
	 * @param saludo Cadena de texto que contiene el saludo
	 */
	void saludar(String saludo){
		System.out.println(saludo);
	}
}

---------------------------------------

// ARCHIVO EnviaSaludo.java

package net.mauriciomatamala;

/**
 *
 * Esta clase utiliza la clase {@link Saludo}
 *
 * @author Mauricio Matamala Peinado
 * @version 0.0
 * @see <a href="http://www.mauriciomatamala.net">www.mauriciomatamala.net</a>
 *
 */
public class EnviaSaludo {

	/**
	 *
	 * @param args Argumentos introducidos desde línea de comandos.
	 */
	public static void main(String[] args) {
		Saludo saludo = new Saludo();
		saludo.saludar("Hola mundo");
	}

}

```
### [Información de referencia del código](https://www.jetbrains.com/help/idea/viewing-reference-information.html#Viewing_Reference_Information.xml)

- Para ver la información sobre un símbolo, encima hacer clic en *Ctrl+Shift+I* y se muestra una ventana con su definición.
- Dejando pulsado *Ctrl* y poniendo el puntero encima de un símbolo, aparece una descripción breve.

### [Información de parámetros](https://www.jetbrains.com/help/idea/viewing-reference-information.html#view-parameter-info)
- IntelliJ muestra un popup con los posibles tipos de los parámetros al ir a invocar una función.

### [Pistas de parámetros](https://www.jetbrains.com/help/idea/viewing-reference-information.html#parameter-hints)
- IntelliJ añade nombres de parámetros en las llamadas a métodos por legibilidad.

### [Documentación rápida](https://www.jetbrains.com/help/idea/viewing-reference-information.html#inline-quick-documentation)
- Si nos ponemos sobre un símbolo y hacemos clic en *Ctrl+Q* o bien en *View -> Quick Documentation* se abre un popup con la documentación javadoc disponible.
- Se puede activar por defecto con solo poner el ratón encima en *Settings->Preferences->Editor->General->Other->Show quick documentation on mouse move*
### [Obtener documentación externa](https://www.jetbrains.com/help/idea/viewing-reference-information.html#external-docs)
- Hay que configurar la URL de la documentación: *Project Structure -> SDKs -> Documentation Path -> Símbolo +(URL) -> Aceptar sugerencia -> Aplicar cambios*. Después de esto, la clase *String* (por ejemplo) mostrará mucha información.

### [Obtener información sobre el tipo de un símbolo](https://www.jetbrains.com/help/idea/viewing-reference-information.html#expression-type-info)
 Haciendo clic sobre *Ctrl+Shift+P*  ( o bien en View->Type Info) se obtiene un popup con el tipo.
 
### [Comentarios TODO](https://www.jetbrains.com/help/idea/using-todo.html#Using_TODO.xml)
Ejemplos de comentarios TODO

	//TODO Añadir algo de código útil por aquí
	
	//FIXME Añadir más archivos de clase:
	// - Jugador
	// - NPC
	// - Pollo
	//Tener cuidado con las interfaces (este comentario no entra dentro del FIXME porque no tiene sangría
 
 Para ver los TODO, *View -> Tool Windows -> TODO* o bien *Alt+6*
 
 Se pueden añadir los propios TODO en *Settings -> Editor -> TODO*. En esta sección pulsar + y añadir un patrón como el siguiente
 	
 	\b<pattern string>\b.*

Por ejemplo, se podría añadir el comentario "Optimization"

## Configuración de la ejecución
Se pueden crear diferentes configuraciones de ejecución para un proyecto. Por ejemplo, imaginemos un proyecto con más de un *main*.

	// Archivo Saludo.java
	
	package net.mauriciomatamala;

	import org.jetbrains.annotations.NotNull;

	public class Saludo {
	    public static void main(String[] args) {
		Saludo saludo = new Saludo();
		saludo.saludar("Hola mundo, desde Saludo.");
	    }

	    public void saludar(@NotNull String textoSaludo){
		System.out.println(textoSaludo);
	    }
	}
	
	// -----------------------------------------------
	// Archivo UsuarioSaludo.java
	
	package net.mauriciomatamala;

	public class UsuarioSaludo {
	    public static void main(String[] args) {
		Saludo saludo = new Saludo();
		saludo.saludar("Hola mundo, desde UsuarioSaludo");
	    }
	}

Opciones:

- [Perfiles de ejecución temporales](https://www.jetbrains.com/help/idea/creating-and-saving-temporary-run-debug-configurations.html#Creating_and_Saving_Temporary_Run_Debug_Configurations.xml). Se crean al  ejecutar manualmente cada clase ejecutable. Después quedan disponibles en la *barra de navegación* (junto al martillo). Allí está la opción de guardar una configuración temporal.
- [Crear una configuración de ejecución manualmente](https://www.jetbrains.com/help/idea/creating-and-editing-run-debug-configurations.html#Creating_and_Editing_Run_Debug_Configurations.xml). 
	- Abrir en la barra de navegación el diálogo *Open run/debug configurations* (junto al martillo) y elegir edit configurations. 
	- Clic en + y elegir Application
	- Introducir campos (nombre, clase main). También se puede indicar en Logs un archivo de salida.
- [Crear una configuración de ejecicón compuesta](https://www.jetbrains.com/help/idea/creating-compound-run-debug-configuration.html#Creating_Compound_Run_Debug_Configuration.xml)
	- Abrir en la barra de navegación el diálogo *Open run/debug configurations* (junto al martillo) y elegir edit configurations. 
	- Clic en + y elegir Compound
	- Introducir nombre y añadir las configuraciones de ejeución deseadas.
	
- [Organizar muchas configuraciónes de ejecución](https://www.jetbrains.com/help/idea/creating-folders-and-grouping-run-debug-configurations.html#create-folder-run-config)
	- Dentro del diálogo *Open run/debug configurations* se pueden crear carpetas para organizar las configuraciones.
	
## [Depuración](https://www.jetbrains.com/help/idea/debugging-code.html)
	
### [Puntos de ruptura](https://www.jetbrains.com/help/idea/using-breakpoints.html#Using_Breakpoints.xml)

Para crear un punto de ruptura, hacer clic junto a la línea de código.
Botón derecho para definir propiedades:

- Enabled - para desactivar temporalmente
- Suspend - para detener al pasar por encima o simplemente pasar y emitir un mensaje.
- Condition - permite detener o no el flujo según una condición. Por ejemplo:

```
	if (a == 3){
		System.out.println("Mensaje de control");
		return true;
		}
	else return false;
	// Con esta condición, el flujo se interrumpirá solo si a vale 3. Además, imprime el mensaje.
```	
- Log: "Breakpoint hit" message - muestra un mensaje al pasar.
- Log : Stack trace - imprimir el mensaje "Breakpint hit" al pasar (marcado) o al final de la ejecución (sin marcar).
- Hay más opciones, como:
	-  "Pass count" que detiene el flujo de ejecución tras pasar varias veces.
	-  "Method entry" se activa cuando se entra en el método con un punto de ruptura.
	-  "Method exit" se activa cuando se sale del método.
- [Watchpoints](https://www.jetbrains.com/help/idea/using-breakpoints.html#field_watchpoint): para controlar el valor de una variable sobre la marcha, durante la depuración, en la sección de variables, hacer clic en + y añadir un watchpoint sobre un atributo.

- Evaluación de expresiones: sobre la línea del breakpoint detenido -> clic derecho -> Evaluate expression -> comprobar valor de elemento de un array, por ejemplo.

## [Stepping toolbar](https://www.jetbrains.com/help/idea/debug-tool-window.html#steptoolbar)

- Show Execution Point 
- Step Over: saltar el método invocado en esta línea (si hay llamada) y seguir por la línea siguiente.
- Step into: ejecutar el método invocado en esta línea.
- Force step into: incluso si el método está configurado para [no ser llamado](https://www.jetbrains.com/help/idea/settings-debugger-stepping.html#Settings_Debugger_Stepping.xml), fuerza su llamada.
- Step out: salir del método actual y seguir por donde iba antes de entrar en él.
- Drop frame: interrumpe la ejecución y vuelve al punto inicial del método en ejecución, descartando el marco de ejecución de la pila.
- Run to cursor:  continua la ejecución hasta el punto donde está el cursor (no hace falta punto de ruptura).
- Evaluate expression: evaluar expresión
- Trace Current Stream Chain: permite [seguir la pista a las operaciones relacionadas con la API Stream](https://www.jetbrains.com/help/idea/analyze-java-stream-operations.html).

## Construcción de un jar
File -> Project structure -> Artifacts -> + -> Jar -> From modules with dependenciese -> Ok
Build -> Build artifacts -> Build

Probar el .jar: 
	
		java -jar ruta_al_archivo/archivo.jar

## Importar archivos jar en un proyecto
File -> Project structure -> Modules -> Dependencias -> + -> jars
Desde el *Project tool window* es posible conocer el contenido del jar.


