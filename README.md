# softpizzeria

# Ejercicio No. 1

Este ejercicio introduce los conceptos básicos de salida en consola y uso de variables en **Python** dentro del contexto del desarrollo progresivo de un software para una pizzería. Primero se utiliza la función `print()` para mostrar mensajes de bienvenida al usuario, incorporando el carácter especial `\n` para generar saltos de línea y organizar visualmente la información en la consola. Posteriormente se presenta el concepto de **variables**, almacenando un mensaje de bienvenida en una variable llamada `mensaje` y mostrándolo mediante `print()`. Este enfoque permite comprender cómo separar los datos de la lógica del programa, facilitando que el software sea más claro, flexible y fácil de modificar a medida que se construyen nuevas funcionalidades del sistema de la pizzería.

# Ejercicio No. 2

Este ejercicio introduce la interacción con el usuario en Python mediante la función input(), ampliando el software de la pizzería con un primer menú principal en consola. El programa comienza mostrando un mensaje de bienvenida almacenado en una variable y presentado con print(), utilizando saltos de línea para mejorar la legibilidad. Luego se definen las opciones del menú —gestión de pedidos y gestión de clientes— guardándolas en variables y mostrándolas al usuario. A continuación, input() permite capturar la opción que el usuario escribe desde el teclado, almacenándola en la variable opcionElegida. Finalmente, el programa confirma la selección mostrando el valor ingresado. Este ejercicio introduce un concepto fundamental en el desarrollo de software interactivo: recibir datos del usuario y utilizarlos dentro del flujo del programa.

# Ejercicio No. 3

Este ejercicio introduce el uso de **estructuras condicionales** en Python para que el software de la pizzería pueda **tomar decisiones según la opción seleccionada por el usuario**. Primero se presenta un menú con varias opciones del sistema —gestión de pedidos, clientes, empleados e inventario— almacenadas en variables y mostradas en la consola. Luego, mediante la función `input()`, el programa captura la opción ingresada por el usuario y la guarda en la variable `opcionElegida`. A continuación, se utilizan las sentencias `if`, `elif` y `else` para evaluar el valor introducido y ejecutar una respuesta específica para cada caso. Python analiza estas condiciones en orden y ejecuta el bloque correspondiente a la primera condición verdadera. Si el valor ingresado no coincide con ninguna opción del menú, se ejecuta el bloque `else`. Con este ejercicio los estudiantes aprenden uno de los mecanismos fundamentales de la programación: **controlar el flujo de ejecución del programa mediante decisiones lógicas**.

# Ejercicio No. 4

Este ejercicio introduce el uso de **estructuras de datos y ciclos iterativos** para mejorar la organización del código del software de la pizzería. En lugar de imprimir cada opción del menú manualmente, las opciones se agrupan en una **tupla llamada `menu`**, que permite almacenar varios elementos de forma ordenada y mantenerlos organizados en una sola estructura. Posteriormente, se utiliza un **ciclo `for`** para recorrer cada elemento de la tupla e imprimirlo en la consola, lo que reduce la repetición de código y facilita el mantenimiento del programa. Después de mostrar el menú, el programa solicita al usuario que elija una opción mediante `input()`, y finalmente se utilizan **condicionales (`if`, `elif`, `else`)** para identificar la opción seleccionada y validar si corresponde a una de las disponibles. Con este ejercicio los estudiantes aprenden a **estructurar mejor la información y automatizar tareas repetitivas mediante iteración**.

# Ejercicio No. 5

Este ejercicio introduce el uso del **bucle `while`** para construir un **menú interactivo que permanece activo hasta que el usuario decide salir del programa**. El sistema muestra repetidamente el menú principal de la pizzería mientras la opción elegida sea diferente de `5`, lo que permite al usuario ejecutar múltiples acciones sin tener que reiniciar la aplicación. Las opciones del menú se almacenan en una **tupla**, lo que facilita su organización y permite recorrerlas mediante un **ciclo `for`** para mostrarlas en la consola de forma automática. En cada iteración del bucle, el programa solicita una opción utilizando `input()` y emplea **estructuras condicionales (`if`, `elif`, `else`)** para responder según la selección del usuario. Cuando se elige la opción de salida, la condición del `while` deja de cumplirse y el programa finaliza mostrando un mensaje de despedida. Este ejercicio integra varios conceptos fundamentales —estructuras de datos, ciclos e instrucciones condicionales— para construir un **flujo básico de navegación en una aplicación de consola**.

# Ejercicio No. 6

Este ejercicio introduce la **implementación de un sistema básico de autenticación de usuarios** dentro del software de la pizzería. Primero se definen variables que almacenan las credenciales correctas (`usuarioGuardado` y `claveGuardada`) y se solicita al usuario que ingrese su nombre de usuario mediante `input()`. El programa valida si el usuario ingresado coincide con el registrado utilizando una estructura condicional `if`. Si el usuario es válido, se inicia un proceso de verificación de contraseña controlado mediante un **bucle `while` con límite de intentos**, permitiendo ingresar la clave hasta un máximo de tres veces. Si la contraseña coincide con la almacenada, el sistema concede el acceso y muestra un mensaje de bienvenida; de lo contrario, el contador de intentos se incrementa y se informa al usuario del número de intentos utilizados. Si se superan los tres intentos, el sistema bloquea el acceso. En caso de que el usuario no esté registrado, el programa informa la situación y sugiere realizar un proceso de registro. Con este ejercicio los estudiantes aprenden a **combinar variables, condicionales y bucles para implementar mecanismos básicos de seguridad y control de acceso en una aplicación**.

# Ejercicio No. 7

Este ejercicio introduce el concepto de **funciones en Python** para mejorar la organización y reutilización del código dentro del software de la pizzería. Una función es un bloque de instrucciones que realiza una tarea específica y que puede ejecutarse cuando el programa la necesita. En este caso se define la función `registrarUsuario()`, que solicita al usuario un nuevo nombre de usuario y una clave, y luego devuelve estos valores mediante la instrucción `return` para que puedan ser utilizados en el programa principal.

El flujo del programa comienza solicitando el nombre de usuario. Si el usuario coincide con el almacenado, el sistema procede a validar la contraseña mediante un **bucle `while` que permite hasta tres intentos**, utilizando condicionales para verificar si la clave ingresada es correcta. Si la contraseña coincide, el acceso es concedido; de lo contrario, el contador de intentos aumenta hasta alcanzar el límite permitido.

Si el usuario ingresado no coincide con el registrado, el programa informa que el usuario no existe y llama a la función `registrarUsuario()` para crear nuevas credenciales. De esta forma, el ejercicio muestra cómo **estructurar programas más grandes utilizando funciones**, mantener el código más organizado y facilitar la reutilización de bloques de lógica dentro de una aplicación interactiva.

# Ejercicio No. 8

Este ejercicio introduce el manejo de **errores y validación de datos** para hacer el software más robusto y evitar que el programa se detenga cuando el usuario ingresa información incorrecta.

En primer lugar, se utiliza la estructura **`try` y `except`**, que permite capturar errores que ocurren durante la ejecución del programa. En este caso, cuando el sistema espera un número entero para la clave, se intenta convertir la entrada del usuario usando `int()`. Si el usuario escribe algo que no es un número, Python genera un error `ValueError`. Gracias al bloque `except`, el programa captura ese error y muestra un mensaje indicando que debe ingresarse un número entero, evitando que el programa se cierre inesperadamente.

El ejercicio también incorpora **validación de datos** para mejorar la seguridad del sistema. El nombre de usuario puede ser cualquier texto, pero la clave debe ser un **número entero de cuatro dígitos**. Para garantizarlo, se verifica que el número esté dentro del rango entre 1000 y 9999. Si el valor ingresado no cumple esta condición, el sistema muestra un mensaje de error y vuelve a solicitar la clave.

En el flujo del programa, primero se intenta iniciar sesión solicitando el usuario. Si el usuario coincide con el almacenado, se procede a validar la clave con un máximo de **tres intentos**, utilizando un bucle `while`. Si el usuario no existe, el programa pregunta si desea registrarse. En caso afirmativo, se llama a la función `registrarUsuario()` para crear un nuevo usuario y una nueva clave con las mismas reglas de validación.

Este ejercicio muestra cómo combinar **funciones, bucles, condicionales, manejo de excepciones y validación de datos** para construir programas interactivos más confiables, acercándose cada vez más a la lógica que tendría un sistema real de software.

# Ejercicio No. 9

Este ejercicio introduce el uso de **diccionarios en Python**, una estructura de datos fundamental para representar información organizada mediante pares **clave–valor**. A diferencia de las listas o tuplas, los diccionarios permiten acceder a los datos mediante una clave específica, lo que facilita estructurar información compleja, como los datos de un usuario dentro de un sistema.

En el primer ejemplo se muestra un diccionario simple llamado `usuario`, donde cada campo del usuario —como `nombre_usuario`, `clave`, `nombre`, `id`, `correo` y `celular`— se almacena como un par clave–valor. Esto permite acceder fácilmente a cualquier dato del usuario utilizando su clave correspondiente, por ejemplo `usuario["nombre"]`.

Posteriormente, el ejercicio presenta una estructura más completa para manejar múltiples usuarios mediante un diccionario llamado `baseUsuarios`. En este caso, el diccionario principal funciona como una **base de datos en memoria**, donde cada clave corresponde al `nombre_usuario` y su valor asociado es otro diccionario que contiene todos los datos de ese usuario. Este enfoque permite organizar múltiples registros de manera estructurada.

La función `registrarUsuario()` se encarga de solicitar al usuario toda la información necesaria para crear un nuevo registro: nombre de usuario, clave de cuatro dígitos, nombre completo, número de identificación, correo electrónico y número de celular. Durante este proceso se aplican validaciones, por ejemplo asegurando que la clave tenga exactamente cuatro dígitos y que el número de identificación sea un valor entero. Finalmente, la función construye y devuelve un diccionario con todos los datos del usuario.

En el programa principal se verifica primero si la base de usuarios está vacía. Si no existen registros, el sistema obliga a crear el **primer usuario del sistema**, garantizando que la base de datos inicial tenga al menos un registro. Ese usuario se almacena en `baseUsuarios` utilizando su nombre de usuario como clave.

Finalmente, el programa recorre el diccionario completo usando `for clave, valor in baseUsuarios.items()`, lo que permite mostrar todos los usuarios registrados y la información asociada a cada uno. Este ejercicio introduce un concepto esencial en el desarrollo de software: **la gestión estructurada de datos**, que es la base para construir sistemas más complejos como bases de datos, sistemas de autenticación y aplicaciones empresariales.

# Ejercicio No. 101

Este ejercicio introduce el concepto de **persistencia de datos en archivos**, permitiendo que la información de los usuarios no se pierda cuando el programa termina su ejecución. En lugar de almacenar los datos únicamente en memoria mediante diccionarios, el sistema ahora guarda y recupera la información desde un archivo en el disco utilizando el formato **CSV (Comma Separated Values)**.

Un archivo CSV es un archivo de texto donde cada línea representa un registro y los campos se separan mediante comas. Este formato es ampliamente utilizado para almacenar datos estructurados porque es simple, legible y compatible con múltiples herramientas, como hojas de cálculo y bases de datos. Para facilitar su manejo, Python proporciona el **módulo `csv`**, que permite leer y escribir este tipo de archivos de manera organizada.

El programa utiliza varias funciones para estructurar el sistema:

* **`cargarUsuarios()`**
  Esta función intenta leer el archivo `baseUsuarios.csv`. Utiliza `csv.DictReader` para convertir cada fila del archivo en un diccionario. Cada usuario se almacena dentro del diccionario `usuarios`, utilizando el `nombre_usuario` como clave. Además, se convierten algunos campos como `clave` e `id` a valores enteros para mantener consistencia en los tipos de datos. Si el archivo no existe, se captura la excepción `FileNotFoundError` y se informa que el archivo será creado cuando se registre el primer usuario.

* **`guardarUsuarios()`**
  Esta función escribe todos los usuarios en el archivo CSV utilizando `csv.DictWriter`. Primero se escriben los nombres de las columnas mediante `writeheader()`, y luego cada usuario se guarda como una fila del archivo. De esta forma, cualquier cambio en la base de usuarios queda almacenado permanentemente.

* **`registrarUsuario()`**
  Permite crear un nuevo usuario solicitando los datos principales del sistema: nombre de usuario, clave de cuatro dígitos, nombre completo, número de identificación, correo electrónico y celular. La clave debe confirmarse dos veces y cumplir con la condición de tener exactamente cuatro dígitos numéricos. Este proceso incluye validaciones mediante `try/except` para evitar errores cuando el usuario ingresa datos inválidos.

* **`login()`**
  Implementa el sistema de autenticación. El usuario ingresa su nombre de usuario y, si existe en la base de datos, debe introducir la clave correcta con un máximo de tres intentos. Si el usuario no existe, el sistema ofrece la posibilidad de registrarlo inmediatamente y guardar sus datos en el archivo CSV.

* **`menuPrincipal()`**
  Una vez autenticado, el usuario accede a un menú interactivo que representa los módulos principales del software de la pizzería: gestión de pedidos, clientes, empleados e inventario. El menú se ejecuta dentro de un bucle `while`, permitiendo seleccionar diferentes opciones hasta que el usuario decide salir del sistema.

En el **programa principal**, primero se cargan los usuarios desde el archivo CSV, luego se ejecuta el proceso de autenticación y, si el inicio de sesión es exitoso, se muestra el menú principal.

Este ejercicio introduce varios conceptos fundamentales en el desarrollo de software:

* Uso de **diccionarios para modelar datos estructurados**.
* Manejo de **archivos CSV para almacenar información persistente**.
* Implementación de **login y registro de usuarios**.
* Uso de **funciones para modularizar el programa**.
* Aplicación de **manejo de errores con `try/except`**.
* Construcción de **interfaces interactivas mediante bucles y menús**.

En conjunto, estos elementos constituyen la base para desarrollar aplicaciones más completas, donde los datos del sistema se conservan entre ejecuciones y el usuario puede interactuar con diferentes módulos del software.
