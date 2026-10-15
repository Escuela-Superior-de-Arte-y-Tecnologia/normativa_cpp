# Normativa de programación ESAT en C y C++ Edición 2026

- [Cómo utilizar esta normativa](#cómo-utilizar-esta-normativa)
- [1. Nomenclatura](#1-nomenclatura)
  - [1.1 Reglas generales de nomenclatura](#11-reglas-generales-de-nomenclatura)
  - [1.2 Nombres de fichero](#12-nombres-de-fichero)
  - [1.3 Nombres de tipos, estructuras y clases](#13-nombres-de-tipos-estructuras-y-clases)
  - [1.4 Nombres de variables](#14-nombres-de-variables)
  - [1.5 Nombres de constantes](#15-nombres-de-constantes)
  - [1.6 Nombres de funciones](#16-nombres-de-funciones)
  - [1.7 Nombres de namespaces](#17-nombres-de-namespaces)
  - [1.8 Nombres de enumeraciones](#18-nombres-de-enumeraciones)
- [2. Formato](#2-formato)
  - [2.1 Longitud de línea](#21-longitud-de-línea)
  - [2.2 Caracteres no ASCII](#22-caracteres-no-ascii)
  - [2.3 Espacios VS tabulaciones](#23-espacios-vs-tabulaciones)
  - [2.4 Formato de las funciones](#24-formato-de-las-funciones)
  - [2.5 Llamadas a función](#25-llamadas-a-función)
  - [2.6 Condicionales](#26-condicionales)
  - [2.7 Bucles y switch](#27-bucles-y-switch)
  - [2.8 Punteros y referencias](#28-punteros-y-referencias)
  - [2.9 Expresiones booleanas](#29-expresiones-booleanas)
  - [2.10 return](#210-return)
  - [2.11 Directivas de preprocesador](#211-directivas-de-preprocesador)
  - [2.12 Formato de clases](#212-formato-de-clases)
  - [2.13 Inicializadores en los constructores](#213-inicializadores-en-los-constructores)
  - [2.14 Namespaces](#214-namespaces)
- [3. Cabeceras](#3-cabeceras)
  - [3.1 Guarda](#31-guarda)
  - [3.2 Declaración por adelantado (forward declaration)](#32-declaración-por-adelantado-forward-declaration)
  - [3.3 Funciones inline](#33-funciones-inline)
  - [3.4 Orden de los parámetros de las funciones](#34-orden-de-los-parámetros-de-las-funciones)
  - [3.5 Nombre y orden de los #include](#35-nombre-y-orden-de-los-include)
- [4. Ámbitos](#4-ámbitos)
  - [4.1 Namespaces](#41-namespaces)
  - [4.2 Clases anidadas](#42-clases-anidadas)
  - [4.3 Funciones locales a un namespace, métodos estáticos y funciones globales](#43-funciones-locales-a-un-namespace-métodos-estáticos-y-funciones-globales)
  - [4.4 Variables locales](#44-variables-locales)
  - [4.5 Variables globales y variables estáticas](#45-variables-globales-y-variables-estáticas)
- [5. Clases](#5-clases)
  - [5.1 Código en los constructores](#51-código-en-los-constructores)
  - [5.2 Constructor por defecto e inicialización de los atributos](#52-constructor-por-defecto-e-inicialización-de-los-atributos)
  - [5.3 Clases copiables / movibles](#53-clases-copiables-movibles)
  - [5.4 struct VS class](#54-struct-vs-class)
  - [5.5 Herencia y composición](#55-herencia-y-composición)
  - [5.6 Herencia múltiple](#56-herencia-múltiple)
  - [5.7 Sobrecarga de operadores](#57-sobrecarga-de-operadores)
  - [5.8 Acceso a datos](#58-acceso-a-datos)
  - [5.9 Orden de declaraciones](#59-orden-de-declaraciones)
  - [5.10 Escribir funciones cortas](#510-escribir-funciones-cortas)
- [6. Particularidades de C++ y C++11](#6-particularidades-de-c-y-c11)
  - [6.1 Parámetros por referencia](#61-parámetros-por-referencia)
  - [6.2 Sobrecarga de funciones y métodos](#62-sobrecarga-de-funciones-y-métodos)
  - [6.3 Valores por defecto para los parámetros de las funciones y métodos](#63-valores-por-defecto-para-los-parámetros-de-las-funciones-y-métodos)
  - [6.4 Lista de argumentos variables y alloca()](#64-lista-de-argumentos-variables-y-alloca)
  - [6.5 friend](#65-friend)
  - [6.6 Excepciones y RTTI](#66-excepciones-y-rtti)
  - [6.7 Casting](#67-casting)
  - [6.8 Streams](#68-streams)
  - [6.9 Pre-incremento y pre-decremento](#69-pre-incremento-y-pre-decremento)
  - [6.10 Uso de const](#610-uso-de-const)
  - [6.11 Tipos enteros](#611-tipos-enteros)
  - [6.12 Macros](#612-macros)
  - [6.13 Representación del cero: 0 y nullptr](#613-representación-del-cero-0-y-nullptr)
  - [6.14 sizeof](#614-sizeof)
  - [6.15 Inicializador con llaves](#615-inicializador-con-llaves)
  - [6.16 Ranged-based for](#616-ranged-based-for)
  - [6.17 auto](#617-auto)
  - [6.18 Uso de constexpr](#618-uso-de-constexpr)
  - [6.19 std::array](#619-stdarray)
- [7. Comentarios](#7-comentarios)
  - [7.1 Estilo de comentario y Doxygen](#71-estilo-de-comentario-y-doxygen)
  - [7.2 Comentarios de fichero](#72-comentarios-de-fichero)
  - [7.3 Comentarios de clases](#73-comentarios-de-clases)
  - [7.4 Comentarios de funciones y métodos](#74-comentarios-de-funciones-y-métodos)
  - [7.5 Comentarios de implementación](#75-comentarios-de-implementación)
  - [7.6 Comentarios de parámetros](#76-comentarios-de-parámetros)
  - [7.7 Sobrecomentar](#77-sobrecomentar)
  - [7.8 TODO y DEPRECATED](#78-todo-y-deprecated)
- [8. Repositorios y proyectos de código](#8-repositorios-y-proyectos-de-código)
  - [8.1 Nombre de los repositorios](#81-nombre-de-los-repositorios)
  - [8.2 Estructura de los directorios de un proyecto](#82-estructura-de-los-directorios-de-un-proyecto)
  - [8.3 Warnings](#83-warnings)

---


> [!NOTE]
> **Cómo interpretar las alertas**
> - **TIP**: ejemplo correcto o recomendación práctica.
> - **CAUTION**: ejemplo incorrecto.
> - **NOTE**: ejemplo neutro o aclaración.
> - **IMPORTANT**: regla fundamental.
> - **WARNING**: advertencia o restricción relevante.

## Cómo utilizar esta normativa

Este documento recoge las normas de programación de la edición 2026. Los ejemplos de código se presentan en bloques Markdown para facilitar su lectura y copia.

## 1. Nomenclatura

Esta sección describe las normas para poner nombre a los elementos del código fuente: las variables, las funciones, las estructuras, las clases, los ficheros, etc...

Todo el código fuente debe ser escrito y comentado **EN INGLÉS** manteniendo un juego de caracteres standard ASCII-7 (esto es, sin ñ, vocales acentuadas, ç y otros símbolos).

### 1.1 Reglas generales de nomenclatura

Los nombres de funciones, variables y ficheros deben ser descriptivos. Se deben evitar abreviaturas innecesarias.

Es mucho más importante que el código sea legible que ahorrar espacio horizontal. No se deben usar abreviaturas ambiguas, que no sean familiares a un nuevo programador que se incorpora al proyecto o forzadas quitando letras a una palabra.

> [!CAUTION]
> **Ejemplo incorrecto**
>
> ```cpp
> // BAD NAMES
> int n;                // Meaningless
> int nerr;             // Ambiguous abbreviation
> int n_comp_conns;     // Ambiguous abbreviation
> int wgc_connections;  // Only your group knows what this is
> int pc_reader;        // Lots of things can be a "pc"
> int cstmr_id;         // Deletes internal letters
> ```

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> // GOOD NAMES
> int price_count_reader;   // No abbreviation
> int num_errors;           // "num" is a widespread convention
> int num_dns_connections;  // Most people know what "DNS" is
> ```

### 1.2 Nombres de fichero

Todos los ficheros deben nombrarse **EN MINÚSCULAS** usando sólo caracteres ASCII-7 y pueden incluir subguiones (_) o guiones (-) en sus nombres. **NUNCA DEBEN INCLUIR ESPACIOS EN BLANCO**:

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> // GOOD - Valid filenames
> my_useful_class.cc
> my-useful-class.cc
> myusefulclass.cc
> myusefulclass_test.cc
> ```

Los ficheros de código C deben tener la extensión .c , los de código C++ deben tener la extensión .cc (a no ser que se estén integrando en un motor que exija otra extensión) y los ficheros de cabecera la extensión .h . Los ficheros que vayan a ser incluidos textualmente por el pre-procesador (e.g: en una compilación multi- plataforma) pueden llevar el sufijo .inc .

No se deben usar nombres de fichero conocidos, como por ejemplo string.h .

En general los nombres deben ser muy específicos. Por ejemplo, se debe usar “http_server_logs.h” en vez de sólo “logs.h” .

Un caso común es nombrar ficheros por parejas, por ejemplo, foo_bar.h y foo_bar.cc para definir e implementar la clase FooBar.

Las funciones implementadas como inline deben ir en el fichero .h tras el bloque class.

### 1.3 Nombres de tipos, estructuras y clases

Los nombres de tipos empiezan con una letra mayúsucula y tienen una mayúscula al principio de cada nueva palabra, sin subguiones: MyExcitingClass, MyExcitingEnum. Los nombres de todos los tipos - y clases, structs, typedefs y enums - siguen la misma convención anterior:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> // classes and structs
> struct UrlTableProperties { ... }
> class UrlTable { ... }
> class UrlTableTester { ... }
>
> // typedefs
> typedef hash_map&lt;UrlTableProperties*, std::string&gt; PropertiesMap;
>
> // enums
> enum UrlTableErrors { ... }
> ```

### 1.4 Nombres de variables

Los nombres de variables y atributos se escriben siempre en minúsculas con subguiones entre palabras. Adicionalmente, los atributos de clase (pero no de struct) acaban en subguión. Por ejemplo: a_local_variable, a_struct_data_member, a_class_data_member_ .

> [!CAUTION]
> **Ejemplo incorrecto**
>
> ```cpp
> std::string tableName;   // Bad - mixed case
> ```

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> std::string table_name;  // OK - uses underscore.
> ```

Las variables globales deben ir prefijadas con “g_” para diferenciarlas del resto.

> [!CAUTION]
> **Ejemplo incorrecto**
>
> ```cpp
> int num_enemies = 8;   // Bad - not starting with g_
>
> void count_enemies() {
>   int num_enemies = 0; // Confusing
>   ...
> }
> ```

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> int g_num_enemies = 8;  // OK
>
> void count_enemies() {
>   int num_enemies = 0; // OK
>   ...
> }
> ```

Las variables de una struct se llaman igual que el resto de variables (no tienen un subguión al final del nombre):

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> struct UrlTableProperties {
>   std::string name;
>   int num_entries;
>   static Pool&lt;UrlTableProperties&gt;* pool;
> };
> ```

Los atributos de clase no-estáticos se llaman igual que el resto de variables, pero acabando en subguión. Las variables estáticas y los atributos de clase estáticos comienzan su nombre con el prefijo s_ :

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> class TableInfo {
>   ...
>  private:
>   std::string table_name_;  // OK - underscore at end.
>   std::string tablename_;   // OK.
>   static Pool&lt;TableInfo&gt;* s_pool_;  // OK.
> };
> ```

### 1.5 Nombres de constantes

Se debe usar una “k” minúscula seguida de una mayúscula por cada palabra, como por ejemplo kDaysInAWeek, para constantes definidas globalmente o dentro de una clase.

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> const int kDaysInAWeek = 7;
> ```

### 1.6 Nombres de funciones

Las funciones normales deben empezar con letra mayúscula y tener una mayúscula por cada nueva palabra, sin subguiones:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> AddTableEntry();
> DeleteUrl();
> OpenFileOrDie();
> ```

Los métodos estáticos de una clase también siguen esta nomenclatura.

Los métodos accessors y mutators (i.e. getters y setters) deben reflejar el nombre del atributo al que acceden. El accessor (getter) debe llamarse como el atributo menos el subguión final. El mutator (setter) debe comenzar por “set_” y seguir con el nombre del atributo sin el subguión final.

El resto de métodos de una clase (que no son estáticos ni accessors ni mutators) se nombrarán empezando por una letra minúscula, sin usar subguiones, poniendo una letra mayúscula al cambiar de palabra, como por ejemplo: init(), finish(), onEnter() .

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> class MyClass {
>  public:
>   ...
>   void init();
>   void onEnter();
>
>   static MyClass* CreateInstance();
>
>   int num_entries() const { return num_entries_; }
>   void set_num_entries(int num_entries) {
>     num_entries_ = num_entries;
>   }
>
>  private:
>   int num_entries_;
> };
> ```

### 1.7 Nombres de namespaces

Los namespaces deben estar en minúscula y basarse en el nombre (y posiblemente ruta) del proyecto (e.g: edk, edk::audio . . . ) .

### 1.8 Nombres de enumeraciones

Las enumeraciones normales se nombran de manera similar a las constantes: el tipo en sí se nombra siguiendo las reglas de nombrado de tipos, empezando por mayúscula y poniendo una mayúscula al comienzo de cada palabra; cada uno de los valores se nombra como una constante, con la salvedad de que después de la “k” se insertan como prefijo el nombre de tipo y un subguión seguido del nombre del valor:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> enum UrlTableErrors {
>   kUrlTableErrors_OK = 0,
>   kUrlTableErrors_ErrorOutOfMemory,
>   kUrlTableErrors_ErrorMalformedInput,
> };
> ```

Las enumeraciones de tipado fuerte (enum class) de C++11 también se nombran de manera similar a las constantes, pero no es necesario insertar el prefijo. El uso de este tipo de enumeraciones es preferible siempre que sea posible:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> enum class UrlTableErrors {
>   k_OK,
>   k_ErrorOutOfMemory,
>   k_ErrorMalformedInput
> };
>
> ...
>
> UrlTableErrors error = UrlTableErrors::k_OK;
> ```

## 2. Formato

Esta sección describe las normas de formato de texto que el código fuente debe seguir, con independencia de qué editor de texto o IDE se use para el desarrollo.

### 2.1 Longitud de línea

> [!IMPORTANT]
> Cada línea de texto de un fichero debe tener como mucho 80 caracteres de longitud. Se recomienda el uso de opciones y plug-ins de los editores de código para marcar una guía visual en esa columna.

### 2.2 Caracteres no ASCII

El uso de caracteres no ASCII debe evitarse. Si no hay más remedio que usarlos, se

debe usar una codificación UTF-8.

### 2.3 Espacios VS tabulaciones

> [!IMPORTANT]
> Se usarán SÓLO espacios, con una indentación standard de 2 espacios. Se debe configurar el editor de código para que emita espacios cuando se pulse el tabulador.

### 2.4 Formato de las funciones

El tipo devuelto estará en la misma línea que el nombre de la función, así como los parámetros y la apertura de llave:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> ReturnType ClassName::functionName(Type par_name1, Type par_name2) {
>   DoSomething();
>   ...
> }
>
> void Character::attackEnemy(Enemy* target, bool critical) {
>   ...
> }
> ```

Si el texto no cabe en una sola línea, se puede partir la lista de parámetros:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> ReturnType ClassName::reallyLongFunctionName(Type par_name1, Type par_name2,
>                                              Type par_name3) {
>   DoSomething();
>   ...
> }
> ```

O incluso:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> ReturnType LongClassName::reallyReallyReallyLongFunctionName(
>     Type par_name1,  // 4 space indent
>     Type par_name2,
>     Type par_name3) {
>   DoSomething();  // 2 space indent
>   ...
> }
> ```

Algunas notas:

- Si el tipo devuelto y el nombre de la función no caben en la misma línea, introducir un salto de línea entre ellos
- Si el salto está después del tipo devuelto, no añadir indentación a la siguiente línea
- Siempre se abre el paréntesis en la misma línea en la que está el nombre de la

función

- Nunca hay un espacio entre el nombre de la función y el paréntesis
- Nunca hay un espacio entre el paréntesis y los parámetros
- Se abre llave al final de la línea en la que esté el último parámetro
- Se cierra llave en una línea aparte en la que no hay nada más (a no ser que la

función sea tan pequeña que toda ella quepa en una línea)

- Todos los parámetros deben tener exactamente los mismos nombres en la

declaración y en la implementación

- Todos los parámetros deben estar alineados
- La indentación por defecto es 2 espacios
- Si los parámetros no caben en la primera línea, su indentación en líneas inferiores

es de 4 espacios

### 2.5 Llamadas a función

Para las llamadas a función, o bien se escribe toda la llamada en un misma línea, o bien se introduce un salto de línea al abrir el paréntesis y se continúa debajo con una indentación de 4 espacios:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> bool retval = DoSomething(argument1, argument2, argument3);
> ...
>
> if (...) {
>   ...
>   ...
>   if (...) {
>     DoSomething(
>         argument1, argument2,  // 4 space indent
>         argument3, argument4);
>   }
> }
> ```

En ocasiones, hay un parámetro especialmente más complejo que el resto que requiere más espacio y una explicación especial:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> bool retval = DoSomething(scores[x] * y + bases[x],  // Heuristic
>                           x, y, z);
> ```

En otras ocasiones, los parámetros forman una estructura que tiene sentido en sí misma (e.g: una matriz):

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> // Transform the widget by a 3x3 matrix.
> my_widget.Transform(x1, x2, x3,
>                     y1, y2, y3,
>                     z1, z2, z3);
> ```

### 2.6 Condicionales

Las instrucciones if y else deben ir en líneas separadas. Las llaves se abrirán al final de la línea en la que está la condición (en el caso del if) o el else. Las instrucciones, la condición y las llaves estarán separadas por un espacio. Si sólo incluyen una instrucción y todo el bloque cabe y se escribe en una sola línea, pueden no usar las llaves, pero en general todo bloque if **DEBE** usar llaves.

Se considera una buena práctica el comenzar una comparación con el valor literal, para evitar errores en los que se escribe una asignación en lugar de una comparación:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> if (5 == condition) {  // no spaces inside parentheses
>   ...  // 2 space indent
> } else if (...) {  // The else goes here
>   ...
> } else { ...
> }
> ```

Los condicionales cortos pueden ser escritos en una sola línea para mejorar la legibilidad, pero sólo si no incluyen else:

> [!CAUTION]
> **Ejemplo incorrecto**
>
> ```cpp
> // BAD -  If statement on one line when there is an ELSE
> if (x) DoThis();
> else DoThat();
> ```

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> // GOOD
> if (kFoo == x) return new Foo();
> if (kBar == x) return new Bar();
> ```

Se indenta con 2 espacios aunque sólo haya una instrucción:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> if (true == condition) {
>   DoSomething();  // 2 space indent.
> }
> ```

### 2.7 Bucles y switch

Las construcciones switch deben usar llaves para delimitar cada caso. Si hay casos agrupados (fall-through), deben ser destacados (por ejemplo, con un comentario). Del mismo modo, debe haber un caso default al final del switch. Si ese caso no debería ejecutarse nunca, se debe colocar un assert en su cuerpo:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> switch (var) {
>   case 0: {  // 2 space indent
>     ...      // 4 space indent
>     break;
>   }
>   case 1: {
>     ...
>     break;
>   }
>   default: {
>     assert(false);
>   }
> }
> ```

En los bucles, la apertura de las llaves debe estar en la misma línea que la condición. Si no contienen código, las llaves se cierran inmediatamente después de abrirse. Nunca se debe omitir el cuerpo del bucle:

> [!CAUTION]
> **Ejemplo incorrecto**
>
> ```cpp
> // BAD -  looks like part of do/while loop.
> while (condition);
> ```

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> // GOOD - empty body.
> while (condition) {
>   // Repeat test until it returns false.
> }
> for (int i = 0; i &lt; kSomeNumber; ++i) {}
> ```

En los nuevos ranged for de C++11, siempre dejamos un espacio antes y después de los dos puntos:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> for (auto i : v) {}
> ```

### 2.8 Punteros y referencias

Al escribir punteros y referencias, no se dejan espacios entre la flecha o el punto y su campo. Del mismo modo, no se dejan espacios tampoco entre * o & y la variable:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> x = *p;
> p = &amp;x;
> x = r.y;
> x = r-&gt;y;
> ```

Cuando se declaran variables puntero o referencia, es indiferente si el símbolo * o & está junto al tipo o el nombre de la variable, pero no debe estar separado de ambos a la vez por espacios:

> [!CAUTION]
> **Ejemplo incorrecto**
>
> ```cpp
> // BAD -  spaces on both sides of *
> char * c;
> // BAD - spaces on both sides of &
> const std::string &amp; str;
> // BAD - multiple variables declared on the same line
> char* c, *d, *e, f;
> ```

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> // GOOD - space preceding
> char *c = nullptr;
> const std::string &amp;str;
>
> // GOOD - space following.
> char* c = nullptr;
> const std::string&amp; str;
> ```

### 2.9 Expresiones booleanas

Cuando se escriban expresiones booleanas que no quepan en una misma línea, se deben partir por el operador lógico que las une:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> if (this_one_thing &gt; this_other_thing &amp;&amp;
>     a_third_thing == a_fourth_thing &amp;&amp;
>     yet_another &amp;&amp; last_one) {
>   ...
> }
> ```

### 2.10 return

No se debe parentizar el return, a no ser que se devuelva el resultado de una expresión compuesta:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> return (value);      // You wouldn't write var = (value);
> return(result);      // return is not a function!
> ```

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> // No parentheses in the simple case
> return result;
> // Parentheses OK to make a complex expression more readable
> return (some_long_condition &amp;&amp;
>         another_condition);
> ```

### 2.11 Directivas de preprocesador

Aunque una directiva de preprocesador (e.g: #if DEBUG) esté a mitad de un bloque indentado, en líneas generales, no estará indentada, comenzará al principio de la línea. En ficheros de configuración donde todo el contenido sean directivas de preprocesador, está permitido indentarlas:

> [!CAUTION]
> **Ejemplo incorrecto**
>
> ```cpp
> // BAD - indented directives
>   if (lopsided_score) {
>     #if DISASTER_PENDING  // Wrong! Should be at beginning of line
>     DropEverything();
>     #endif                // Wrong! Do not indent "#endif"
>     BackToNormal();
> }
> ```

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> // GOOD - directives at beginning of line
>   if (lopsided_score) {
> #if DISASTER_PENDING
>     DropEverything();
> # if NOTIFY
>     NotifyClient();
> # endif
> #endif
>     BackToNormal();
>   }
> ```

### 2.12 Formato de clases

El nombre de la clase y de la clase madre deben estar en la misma línea (la primera) si el ancho de línea lo permite.

Las palabras clave public: , protected: y private: sólo llevan 1 espacio de indentación, van precedidas de una línea en blanco (excepto en la primera ocurrencia) y van en el orden recién descrito:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> class MyClass : public OtherClass {
>  public:      // Note the 1 space indent!
>   MyClass();  // Regular 2 space indent.
>   explicit MyClass(int var);
>   ~MyClass() {}
>
>   void someFunction();
>   void someFunctionThatDoesNothing() {}
>
>   void set_some_var(int var) { some_var_ = var; }
>   int some_var() const { return some_var_; }
>
>  private:
>   bool someInternalFunction();
>
>   int some_var_;
>   int some_other_var_;
> };
> ```

### 2.13 Inicializadores en los constructores

Las listas de inicializadores en un constructor se pueden escribir de dos formas distintas: en una sola línea o separadas en múltiples líneas colocando los dos puntos en la primera línea de los inicializadores con una indentación de 4 espacios:

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> // GOOD - When it all fits on one line:
> MyClass::MyClass(int var) : some_var_(var), other_var_(var + 1) {}
>
> // GOOD - When it requires multiple lines, indent 4 spaces,
> // putting the colon on the first initializer line:
> MyClass::MyClass(int var)
>     : some_var_(var),             // 4 space indent
>       other_var_(var + 1) {       // lined up
>   ...
>   DoSomething();
>   ...
>   }
> ```

### 2.14 Namespaces

Abrir un namespace **NO** añade un nivel de indentación. Si se declaran namespaces anidados, cada declaración va en su propia línea:

> [!CAUTION]
> **Ejemplo incorrecto**
>
> ```cpp
> // BAD - Indented when it should not be
> namespace foo {
>   namespace bar {
>     void Paw() {
>       ...
> }
>   }  // namespace bar
> }  // namespace foo
> ```

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> // GOOD - No extra indentation within namespace
> namespace foo {
> namespace bar {
>
> void Paw() {
>   ...
> }
>
> }  // namespace bar
> }  // namespace foo
> ```

## 3. Cabeceras

En general, cada fichero .c ó .cc debe llevar su cabecera .h asociada. Hay algunas excepciones comunes como los test unitarios o ficheros muy pequeños que contienen sólo la función main() .

### 3.1 Guarda

Todas las cabeceras deben tener su correspondiente guarda con #define para

prevenir que se incluyan múltiples veces. El formato de la guarda es:

__FICHERO_H__ 1

Si dentro del mismo proyecto se encuentra dos ficheros de idéntico nombre pero distinta ruta, la ruta se incluirá como parte de la guarda de la siguiente manera:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> #ifndef __ENGINE_H__
> #define __ENGINE_H__ 1
>
> ...
>
> #endif  // __ENGINE_H__
> ```

### 3.2 Declaración por adelantado (forward declaration)

Deben declararse por adelantado clases o structs de los que sólo se referencie su nombre para evitar añadir #include innecesarios.

> [!CAUTION]
> **Ejemplo incorrecto**
>
> ```cpp
> // BAD
> #include “sprite.h”
>
> ...
>
> Sprite* sprite_ptr;
> ```

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> // GOOD
> class Sprite;
>
> ...
>
> Sprite* sprite_ptr = nullptr;
> ```

### 3.3 Funciones inline

En el caso de que por eficiencia se quisiera que una función fuese inline, esta será candidata a ser inline si no sobrepasa las 10 lineas de código.

Las funciones inline deben escribirse en su correspondiente fichero de cabecera después del bloque class (si lo hubiera).

### 3.4 Orden de los parámetros de las funciones

Cuando se defina una función, el orden de los parámetros es el siguiente: primero los de entrada, luego los de salida.

### 3.5 Nombre y orden de los #include

El orden de escritura de los #include será el siguiente:

- La cabecera correspondiente a este archivo
- Cabeceras de C
- Cabeceras de C++
- Otras librerías externas
- Otras cabeceras de este proyecto

## 4. Ámbitos

### 4.1 Namespaces

El uso de namespaces para crear ámbitos es una buena práctica. Los namespaces deben recibir sus nombres en relación al proyecto y su ruta. Debe evitarse la directiva using cuando no sea necesaria. En especial, debe evitarse la directiva “using namespace” , siendo preferible usar sólo using con elementos concretos. Está completamente **PROHIBIDO** el uso de using en una cabecera:

> [!CAUTION]
> **Ejemplo incorrecto**
>
> ```cpp
> // BAD - In a .h file
> #include &lt;string&gt;
>
> using namespace std;    // FORBIDDEN - You are forcing the linkage
>                         // of the whole available namespace symbols
>                         // to anyone who includes this header
> string my_string;
> ```

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> // GOOD - In a .h file
> #include &lt;string&gt;
>
> std::string my_string;  // You are only linking std::string
> ```

En un fichero de código .cc podemos aplicar using a elementos concretos, pero en general es preferible no depender de ello:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> // In a .cc file
> using std::cout;
> using std::endl;
>
> void Foo() {
>   std::cout &lt;&lt; “Foo!” &lt;&lt; std::endl;
> }
> ```

### 4.2 Clases anidadas

El uso de clases anidadas está permitido, pero se recomienda usar namespaces en ese tipo de casos, cuando sea posible.

### 4.3 Funciones locales a un namespace, métodos estáticos y funciones globales

Es preferible usar funciones locales a un namespace o métodos estáticos a usar funciones totalmente globales, para evitar conflictos de nombres de símbolos.

### 4.4 Variables locales

Las variables de una función deben ponerse en el ámbito más cerrado posible, y deben ser inicializadas en la declaración. Sólo se declarará una variable por línea de código.

Las variables declaradas en cada pila deben, en total, mantener un tamaño reducido (e.g: < 4kB). Para necesidades de memoria más grandes se debe usar el heap (o el segmento de datos).

C++ permite declarar variables en cualquier lugar de una función, pero siguiendo esta guía, deben declararse en el ámbito más local posible y tan cerca de su primer uso como sea posible. Esto facilita enormemente la legibilidad y comprensión del código, al mostrar el tipo y valor de la variable en el lugar adecuado:

> [!CAUTION]
> **Ejemplo incorrecto**
>
> ```cpp
> // BAD - initialization separate from declaration
> int i;
> i = f();
> ```

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> // GOOD
> int i = f();
> ```

> [!CAUTION]
> **Ejemplo incorrecto**
>
> ```cpp
> // BAD - Prefer initializing using
> // brace initialization
> std::vector&lt;int&gt; v;
> v.push_back(1);
> v.push_back(2);
> ```

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> // GOOD - v starts initialized
> std::vector&lt;int&gt; v = {1, 2};
> ```

Las variables necesarias para if, while y for normalmente deben ser declaradas dentro de esas estructuras de control dado que están confinadas a esos ámbitos. La excepción serán las variables que sean objetos dado que, por eficiencia, debe evitarse que el constructor se ejecute en cada iteración de un bucle for o while:

> [!CAUTION]
> **Ejemplo incorrecto**
>
> ```cpp
> // BAD - Inefficient implementation:
> for (int i = 0; i &lt; 1000000; ++i) {
>   Foo f;
>   // My constructor and destructor get called
>   // 1000000 times each.
>   f.doSomething(i);
> }
> ```

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> // GOOD - My constuctor and destructor get called
> // only once each
> Foo f;
> for (int i = 0; i &lt; 1000000; ++i) {
>   f.doSomething(i);
>   }
> ```

### 4.5 Variables globales y variables estáticas

El uso de variables estáticas o globales, especialmente las que sean objetos, está **PROHIBIDO**: causan bugs difíciles de encontrar debido al orden indeterminado de construcción y destrucción. Sin embargo, sí están permitidas sin son constantes (constexpr), dado que no tienen inicialización ni destrucción dinámicas.

Los objetos que tengan una duración estática, incluyendo variables estáticas, métodos y atributos estáticos, así como funciones estáticas, deben ser Plain Old Data (POD): sólo int, char, float, double, punteros o arrays de POD. Esta prohibición, por tanto, prohibe el uso de variables globales o estáticas de tipo std::vector (se debe usar un array de C en ese caso), o std::string (se debe usar const char []).

Si parece necesario el uso de una variable estática que sea un objeto, se debe usar un puntero a ese objeto.

El orden en el que se llama a los constructores y destructores de una variable estática está sólo parcialmente especificado en C++ , e incluso puede variar de compilación a compilación, lo que causa bugs muy difíciles de encontrar. Por ello, no se permite tampoco el uso de variables estáticas POD que se inicialicen con el resultado de una función, a no ser que dicha función no dependa de otras globales (como getenv() o getpid() ). Esto no afecta a las variables estáticas declaradas dentro de una función, las cuales sí tienen un orden de inicialización bien definido:

> [!CAUTION]
> **Ejemplo incorrecto**
>
> ```cpp
> // BAD - Global object variables
> class Object;
>
> Object g_my_object;
> ```

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> // GOOD - Global object pointer
> class Object;
>
> Object* g_my_object = nullptr;
> ```

## 5. Clases

### 5.1 Código en los constructores

Se debe evitar escribir código en los constructores que no pertenezca a la inicialización trivial del objeto. En particular, se debe evitar código que pueda fallar o que requiera llamadas a métodos virtuales.

Si un objeto requiere código no trivial, se debe escribir en el método init() :

> [!CAUTION]
> **Ejemplo incorrecto**
>
> ```cpp
> // BAD - Non-trivial constructor
> Object::Object() {
>   attribute_ = 0;
>   FunctionThatCanFail();
>   virtualFunctionThatCanFail();
>   ptr_ = malloc(kALotOfMemory);
> }
> ```

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> // GOOD - Trivial constructor and init method
> Object::Object() {
>   attribute_ = 0;
> }
>
> void Object::init() {
>   FunctionThatCanFail();
>   virtualFunctionThatCanFail();
>   ptr_ = malloc(kALotOfMemory);
> }
> ```

### 5.2 Constructor por defecto e inicialización de los atributos

Si una clase tiene atributos, se debe escribir al menos un constructor que los inicialice (que puede ser el constructor por defecto). Si no se declara un constructor, el compilador creará uno arbitrario, y eso es malo dado que puede dejar el objeto en un estado indeterminado. Marcaremos el constructor por defecto usando el keyword de C++11 =default explícitamente:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> class SomeType {
>   // Explicit default constructor
>   SomeType() = default;
>   SomeType(OtherType value);
>   . . .
> };
> ```

### 5.3 Clases copiables / movibles

Si tiene sentido para una clase, se puede definir un mecanismo de copia. Pero si no tiene sentido, la copia debe estar explicitamente deshabilitada (e.g: con un constructor de copia privado o con el keyword de C++11 =delete ).

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> // The following class is non-copyable
> class NonCopyable {
>   NonCopyable&amp; operator=(const NonCopyable&amp;) = delete;
>   NonCopyable(const NonCopyable&amp;) = delete;
>   ...
>   };
> ```

Si una clase va a ser copiable y no se espera que haya subclases que deriven de ella, se debe implementar un constructor de copia y un operador de asignación.

Si una clase va a ser copiable y sí se espera que haya subclases que deriven de ella, es aconsejable implementar un método público virtual clone() y un constructor de copia protected para que las clases derivadas puedan implementar el clone() .

### 5.4 struct VS class

Se usa struct sólo para los objetos pasivos que llevan datos; todo lo demás es class.

### 5.5 Herencia y composición

La composición es generalmente más apropiada que la herencia. Si hay que

implementar una herencia, siempre debe ser pública.

Si la clase incluye métodos virtuales, su destructor debe ser virtual.

El uso de protected debe estar restringido a aquellos métodos que vayan a ser usados por las subclases.

### 5.6 Herencia múltiple

No está permitida.

### 5.7 Sobrecarga de operadores

En general, la sobrecarga de operadores no está recomendada excepto en casos puntuales. Por eficiencia y evitar confusiones de código, es preferible usar métodos con nombre (e.g: Equals() , Add() . . .) a sobrecargar operadores como == ó + .

En particular, la sobrecarga de operator& y operator” “ está **PROHIBIDA** dado que rompe otras funcionalidades de C++ (i.e. forward declaration y aritmética de punteros).

En los casos en los que la sobrecarga de operadores sea necesaria para interactuar con el API de la STL, o en objetos donde tenga un sentido semántico, la sobrecarga de operadores está permitida.

### 5.8 Acceso a datos

Los atributos de una clase serán generalmente privados y se dará acceso a ellos a través de accessors y mutators (i.e. getters y setters).

Si una variable se llama foo_ , su getter será foo() y su setter set_foo() .

Los atributos static const (e.g: kFoo) no tienen por qué ser privados.

El código de estos métodos suele situarse en la declaración de la clase en el fichero de cabecera, pero no tiene por qué ser así en todos los casos.

### 5.9 Orden de declaraciones

El orden será public después protected y por último private. Si una de estas secciones no va a tener contenido, se omitirá. Dentro de cada sección, se seguirá el siguiente orden:

- typedefs y enums
- Constantes (miembros static const)
- Constructores
- Destructores
- Métodos, incluyendo los estáticos
- Atributos (excepto los static const)

El orden a seguir en el fichero .cc será el mismo, tanto como sea posible.

### 5.10 Escribir funciones cortas

Es preferible escribir funciones cortas, enfocadas y concisas que llevan a cabo una tarea determinada.

Es cierto que en algunos casos una función larga es necesaria, así que no hay un límite duro en la longitud de las funciones. Ahora, si una función excede las 40 líneas, es probable que pueda ser separada en varias funciones sin dañar la estructura del programa.

## 6. Particularidades de C++ y C++11

### 6.1 Parámetros por referencia

Todos los parámetros pasados por referencia (referencias de C++) deben ser const, excepto en aquellos casos en los que el objeto deba ser modificado dentro de la función.

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> void Foo(const std::string&amp; in, std::string* out);
> ```

### 6.2 Sobrecarga de funciones y métodos

Las funciones y métodos (incluyendo constructores) se pueden sobrecargar (i.e. overload, implementar varias versiones de una función con el mismo nombre) sólo si en el API queda claro lo que hace esa función sin tener que consultar todas las sobrecargas.

Antes de sobrecargar una función, hay que considerar cualificar el nombre con información sobre los argumentos. E.g: AppendString() o AppendInt() en vez de sólo Append().

### 6.3 Valores por defecto para los parámetros de las funciones y métodos

En los siguientes casos se permite el uso de valores por defecto a los argumentos:

- Constructores
- Funciones estáticas
- Para simular listas variables de argumentos

En el resto de casos, no es recomendable usar valores por defecto dado que introducen ambigüedad en las signatures de las funciones:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> // Support up to 4 params by using a default
> // empty value
> std::string StrJoin(const char *a,
>     const char* b = nullptr,
>     const char* c = nullptr,
>     const char* d = nullptr);
> ```

### 6.4 Lista de argumentos variables y alloca()

En líneas generales, no es recomendable el uso de las listas de argumentos variables y alloca() .

Ambas técnicas son generalmente eficientes, pero no forman parte del standard de C / C++ y tienen comportamientos diferentes en compiladores diferentes e incluso entre código Debug y Release. De hecho alloca() no suele estar soportado en sistemas Windows. Por tanto, su uso no está recomendado.

### 6.5 friend

El uso de friend está restringido a clases y funciones dentro del mismo fichero .cc y a casos en los que una clase construye objetos de otra (e.g: class FooBuilder , class Foo) o patrones de Singleton.

### 6.6 Excepciones y RTTI

No están permitidas las excepciones de C++ .

### 6.7 Casting

Se deben usar casts de C++ , como static_cast<>() . Se deben evitar casts de C clásicos como  int y = (int)x;  o  int y = int(x);

- Se debe usar static_cast como el equivalente del clásico cast de C que hace conversión de valores, o bien cuando es necesario hacer un up-cast de un puntero de una clase a su clase madre
- Se debe usar const_cast para retirar el calificador const
- NO se debe usar reinterpret_cast (por romper el diseño de código)
- NO se debe usar dynamic_cast (por la desactivación de RTTI)

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> // GOOD - Use of static_cast
> Base * a = new Base;
> Derived * b = static_cast&lt;Derived*&gt;(a);
> ```

Excepto en casos explícitos de optimización en C de bajo nivel, NO se debe usar el casting clásico de C en C++ .

### 6.8 Streams

Se deben usar streams (e.g: ifstream, ofstream) sólo para logs. En otros casos, usar printf() o funciones similares.

### 6.9 Pre-incremento y pre-decremento

Se puede usar la forma de prefijo (++i) o sufijo (i++) de incremento y decremento con iteradores y otros objetos similares. Para variables escalares (no objetos) es indiferente el uso de pre-incremento o post-incremento.

### 6.10 Uso de const

Se debe usar const si:

- Una función no modifica un argumento pasado como referencia o puntero. Ese argumento debe ser const
- Declaramos un método. A no ser que un método cambie el estado del objeto, debe ser const. Los accessors (getters) deben ser const. Todos los métodos que no modifican un objeto deben ser const
- Un atributo no va a ser modificado después de la construcción

### 6.11 Tipos enteros

De los tipos enteros incluidos en C++ , el único usable es int. Si un juego necesita una variable de tamaño distinto, se debe usar un tipo preciso de <stdint.h> o equivalente, como por ejemplo int16_t . Si una variable debe representar un valor que puede ser mayor que 2^31 (2GiB), se deben usar tipos de 64 bits, como int64_t o equivalente.

Cabeceras como <stdint.h> definen tipos precisos portables como int16_t, uint32_t, int64_t, etc... Deben usarse esos tipos en vez de short, unsigned long long, y otros similares que no garantizan el tamaño de la variable en múltiples plataformas.

NO se deben usar tipos unsigned como medida e indicación de que una variable no baje nunca de cero (porque provocará un bug de underflow). Si una variable no debe bajar nunca de cero, se debe usar un assert.

### 6.12 Macros

Las macros deben evitarse en la medida de lo posible. Es preferible usar funciones inline, enums y consts:

> [!CAUTION]
> **Ejemplo incorrecto**
>
> ```cpp
> // BAD - unnecessary use of macros
> #define GetMax(a,b) ((a)&gt;(b)?(a):(b))
> #define ONE     1
> #define TWO     2
> #define THREE   3
> #define MAX_NUM 3
> ```

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> // GOOD
> inline int GetMax(int a, int b) { return a&gt;b?a:b; }
> enum Number {
>   kNumber_One = 1,
>   kNumber_Two,
>   kNumber_Three
> };
> const int kMax_num = 3;
> ```

- No se definen macros en los ficheros .h
- Escribir los #define justo antes de su uso y los #undef justo después
- En vez de usar un #define para una macro de una función corta crítica, usar una función inline
- Definir enums y const en vez de una serie de #define

### 6.13 Representación del cero: 0 y nullptr

Se debe usar 0 para enteros, 0.0f para float, 0.0 para double, nullptr para punteros y ‘\0’ para char.

### 6.14 sizeof

sizeof() debe llamarse generalmente sobre variables en vez de sobre tipos, por si el tipo de una variable cambia en el futuro:

> [!CAUTION]
> **Ejemplo incorrecto**
>
> ```cpp
> // BAD - sizeof over type
> memset(&amp;data, 0, sizeof(MyClass));
> ```

> [!TIP]
> **Ejemplo correcto**
>
> ```cpp
> // GOOD - sizeof over variable
> struct PlayerData data;
> memset(&amp;data, 0, sizeof(data));
> ```

### 6.15 Inicializador con llaves

Se pueden usar inicializadores con llaves en arrays y structs:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> struct Point { int x; int y; };
> Point p = {1, 2};
> ```

Desde C++11, también es posible utilizar la sintaxis de las llaves para inicializar muchos otros tipos de datos (i.e. braced-init-list o initializer_list ) :

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> // Vector takes a braced-init-list of elements
> std::vector&lt;std::string&gt; v{"foo", "bar"};
>
> // Basically the same
> // You may choose to use either form
> std::vector&lt;std::string&gt; v = {"foo", "bar"};
>
> // Usable with 'new' expressions.
> auto p = new std::vector&lt;std::string&gt;{"foo", "bar"};
>
> // A map can take a list of pairs
> // Nested braced-init-lists work
> std::map&lt;int, std::string&gt; m = {{1, "one"}, {2, "2"}};
>
> // A braced-init-list can be implicitly converted
> // to a return type.
> std::vector&lt;int&gt; test_function() { return {1, 2, 3}; }
>
> // Iterate over a braced-init-list.
> for (int i : {-1, -2, -3}) {}
>
> // Call a function using a braced-init-list
> void TestFunction2(std::vector&lt;int&gt; v) {}
> TestFunction2({1, 2, 3});
> ```

### 6.16 Ranged-based for

En C++11 se introduce un nuevo tipo de for que itera sobre los valores de un contenedor de variables, como un array o un std::vector :

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> int a[] = {0, 1, 2, 3, 4, 5};
> for (int n : a) {
>   std::cout &lt;&lt; n &lt;&lt; ” ”;
> }
>
> std::vector&lt;int&gt; v = {0, 1, 2, 3, 4, 5};
> for (auto i : v) {
>   std::cout &lt;&lt; i &lt;&lt; ” ”;
> }
> ```

### 6.17 auto

En C++11 se introduce el uso de auto para indicar un tipo de datos que se deducirá en tiempo de compilación por el contexto. Su uso está permitido en casos donde mejor la legibilidad del código y/o el tipo de una variable no es relevante (ver sección 6.16)

### 6.18 Uso de constexpr

En C++11 se introduce la palabra clave constexpr (expresión constante), que permite al usuario garantizar que una función o un constructor de objeto es constante en tiempo de compilación. El uso de este mecanismo es seguro y está permitido (e.g: para determinar el tamaño de un array):

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> constexpr int GimmeFive() {
>   return 5;
> }
>
> // Creates an array of 12 ints. Legal in C++11
> int an_array[GimmeFive() + 7];
> ```

### 6.19 std::array

En C++11 se introduce el nuevo contenedor de la STL std::array , que viene a ser una versión moderna de los array clásicos de C con mejor integración con otros mecanismos de la STL (i.e: iteradores, algoritmos, etc...) y en la que la mayoría de operaciones se resuelven en tiempo de compilación. El uso de este contenedor es seguro y está permitido, y se puede usar indistintamente en los casos en los que se usaría un array clásico de C:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> std::array&lt;int,10&gt; myarray;
> unsigned int i = 0;
>
> // Assign some values:
> for (i=0; i&lt;10; ++i) myarray[i]=i;
>
> // Print content
> std::cout &lt;&lt; "myarray contains:";
> for (i=0; i&lt;10; ++i) {
>   std::cout &lt;&lt; ' ' &lt;&lt; myarray[i];
> }
> std::cout &lt;&lt; '\n';
> ```

## 7. Comentarios

### 7.1 Estilo de comentario y Doxygen

Se debe usar la sintaxis de o bien // o bien /* */ , mientras se sea consistente. En general todas las clases, funciones, tipos, etc... deben estar correctamente comentados siguiendo la sintaxis de Doxygen, esto es, con bloques de tipo /// para una sola línea o /** */ para un bloque de líneas.

### 7.2 Comentarios de fichero

Se deben comenzar todos los ficheros con un encabezado de comentario en el que se indique el nombre del fichero, una breve descripción de lo que se implementa en él, el autor y la fecha.

Generalmente un fichero .h describirá la clase que tiene declarada y una visión general de para qué sirve y cómo se usa. Un fichero .cc debería incluir más información acerca de detalles de implementación y explicación de los algoritmos. Si se entiende que estas explicaciones son de interés para alguien que sólo va a usar el .h , deben incluirse en él, pero debe indicarse en el .cc que los comentarios están en la cabecera.

NO se deben duplicar comentarios en el .h y en el .cc . Los comentarios duplicados divergen y crean errores de comprensión.

### 7.3 Comentarios de clases

Todas las definiciones de clase (en su .h) deben ir acompañadas por un comentario que describe para qué sirven y cómo se utilizan. El comentario estará situado justo sobre la clase y seguirá la norma y sintaxis de Doxygen.

### 7.4 Comentarios de funciones y métodos

Sobre su declaración, todas las funciones deben tener un comentario explicando para qué sirven y cómo se usan, así como especificando su resultado (si lo devuelven) y sus parámetros (si los tienen) en sintaxis Doxygen (i.e: usando @param , @result y otros comandos Doxygen):

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> /** Delete a URL from the cache
> @result 0 if successful or an error code
> @param url The URL to be deleted
> */
> int DeleteUrl(const char* url);
> ```

### 7.5 Comentarios de implementación

Partes del código complejas o difíciles de entender deben ir precedidas de un comentario explicativo y/o de un esquema claro.

### 7.6 Comentarios de parámetros

Cuando se pase un puntero a nullptr o NULL, un booleano, o valores literales enteros a funciones como parámetros, es aconsejable incluir un comentario explicando lo que son y significan, o bien hacer el código más autoexplicativo usando constantes:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> bool success = Calculate(interesting_value,
>                          10,
>                          false,
>                          nullptr);  // What are these arguments??
> ```

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> bool success = Calculate(interesting_value,
>                          10,        // Default base value
>                          false,     // Not the first time calling
>                          nullptr);  // No callback
> ```

Alternativamente, se pueden usar constantes o variables auto-explicativas:

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> const int kDefaultBaseValue = 10;
> const bool kFirstTimeCalling = false;
> Callback* null_callback = nullptr;
> bool success = CalculateSomething(interesting_value,
>                                   kDefaultBaseValue,
>                                   kFirstTimeCalling,
>                                   null_callback);
> ```

### 7.7 Sobrecomentar

Se debe evitar el comentario excesivo o sobrante (e.g: no todos los bucles deben tener encima un comentario que explique que recorren una estructura de datos) dado que hace la lectura del código más farragosa.

### 7.8 TODO y DEPRECATED

Se deben usar comentarios TODO para marcar código que es temporal, una solución a corto plazo o que es buena de momento, pero no perfecta.

Del mismo modo, se deben usar los comentarios DEPRECATED para marcar partes de un API que van a desaparecer pronto y a las que se ha ofrecido una alternativa (incluida en el comentario):

> [!NOTE]
> **Ejemplo de código**
>
> ```cpp
> // TODO(pepe@gmail.com): Use a "*" here for concat. operator
> // TODO(Luis) change this to use relations
> . . .
> // DEPRECATED(Jose): Please use MyClass::DeleteUrl() now
> ```

## 8. Repositorios y proyectos de código

### 8.1 Nombre de los repositorios

Las reglas para nombrar los repositorios de código son las siguientes:

- Comenzará por un número correspondiente al curso del alumno, i.e., “2” para segundo y “3” para tercero
- Después dos letras mayúsculas que identificarán la asignatura a la que corresponde el repositorio siguiendo la correspondencia:

- Después un subguión y la cadena “MA_” o “TA_” dependiendo de si el alumno es de grupo de mañana o de tardes.
- Por último, en minúsculas, el login del alumno.

Ejemplos: “2PA_MA_garanda”, “3IA_TA_garanda”

### 8.2 Estructura de los directorios de un proyecto

Los directorios de un proyecto en C / C++ deberán seguir una estructura fija predefinida excepto en el caso de que el uso de un motor o framework concreto exija una estructura diferente (e.g: Unreal Engine 4). Dicha estructura es la siguiente:

- bin/ - Ejecutables finales de la compilación
- data/ - Ficheros usados por los ejecutables
- build/ - Ficheros binarios temporales creados durante la compilación (e.g: .obj, .ilk . . .) y scripts de compilación.
- src/ - Ficheros fuente de implementación del proyecto, i.e., acabados en .cc
- include/ - Ficheros de cabecera, i.e., acabados en .h
- doc/ - Documentación del proyecto
- deps/ - Dependencias externas para la compilación del proyecto (e.g: librería ESAT)

### 8.3 Warnings

En la configuración de los proyectos, se deben activar los flags de Warnings al compilar. Pueden ser los Warnings importantes (/W3 en cl) o bien “All Warnings” (que suele ser el parámetro /Wall o -Wall en la mayoría de compiladores) para poder visualizar y resolver todos los warnings de compilación. Ninguna entrega de código debe realizarse con warnings importantes pendientes de resolver.
