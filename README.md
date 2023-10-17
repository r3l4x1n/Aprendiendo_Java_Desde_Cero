# JAVA DESDE CERO
## JDK
El JDK, o Java Development Kit, es una colección de herramientas de software que se utilizan para desarrollar aplicaciones de Java. El JDK incluye un compilador, un depurador, una máquina virtual Java (JVM) y otras herramientas que se utilizan para crear, probar y ejecutar aplicaciones de Java.

## IntelliJ IDEA
[IntelliJ IDEA](https://www.jetbrains.com/help/idea/installation-guide.html) es un entorno de desarrollo integrado (IDE) altamente popular y ampliamente utilizado para el desarrollo de software en lenguajes de programación como Java, Kotlin, Groovy y Scala, entre otros. Desarrollado por JetBrains, IntelliJ IDEA ofrece una amplia gama de herramientas y características avanzadas que ayudan a los programadores a escribir, depurar y mantener código de manera eficiente.

## CLASES
Una [**Clase**](https://www.w3schools.com/java/java_oop.asp) es una *plantilla* que se usa para crear [**Objetos**](https://www.w3schools.com/java/java_classes.asp). Cada objeto puede tener su propio conjunto de características y cosas que puede hacer.
En JAVA, los nombres de las clases deben comenzar con una letra mayúscula y, si son palabras compuestas, cada palabra debe comenzar con una letra mayúscula. Por ejemplo, en la clase "ClaseEjemplo" usamos la convencion (cammelCase).
Además, cuando se crea una clase, el archivo que se crea debe llevar el mismo nombre.

## METODO
En Java, un método se asemeja a una acción. Una acción que una **Clase** puede llevar a cabo. Para ilustrar esto mejor, imagina que tienes un objeto, un "Robot" por ejemplo. Dentro de esta objeto "Robot" se pueden ejecutar acciones como "moverse", "saludar", "bailar" y demás. Cada una de estas acciones que el robot puede llevar a cabo se denomina un [**Método**](https://www.javatpoint.com/method-in-java).
En términos generales, un método es una forma de realizar una tarea específica.

### Metodo main()
El método ```public static void main(String[] args){}``` o metodo *main*, sirve como punto de entrada para la ejecución de un programa Java y corresponde al método principal (main) de una clase. Su propósito principal es permitir que el sistema inicie y ejecute el programa.
https://www.javatpoint.com/java-main-method

## VARIABLES
JAVA es un lenguanje de programacion fuertemente tipado. Esto quiere decir que cualquier variable que se defina en la app, tiene que estar asociada a un tipo de dato.
Para la declaracion de una variable en JAVA, se debe de considerar el "tipo de dato" y el "nombre de la variable".
A partir de JAVA10 se permite el tipado dinamico para definir variables con la palabra "var".

### Reglas Para Definir Variables en JAVA
- Por convencion, los nombres de las variables empiezan con una letra minuscula.
- Debe ser un juego de caracteres comprendidos en la codificacion Unicode. (No puede tener caracteres especiales y no debe comenzar con un numero).
- No debe de tener el mismo nombre que otra variable dentro del mismo ambito.
- Si tenemos palabras compuestas, se deben poner juntas y cada palabra despues de la primera empieza con Mayuscula (camelCase).

En Java, las variables pueden clasificarse en tres categorías principales: locales, de instancia y estáticas. Cada una de estas categorías tiene un alcance y una duración de vida diferente en el programa. A continuación, te explicaré cada tipo de variable:

Variables Locales:
Alcance: Una variable declarada dentro del cuerpo del método se llama variable local. Puede usar esta variable solo dentro de ese método y los otros métodos de la clase ni siquiera saben que la variable existe.
Duración de vida: La variable local existe solo mientras el método o bloque en el que se declara se está ejecutando. Una vez que el método o bloque termina, la variable se destruye y su valor se pierde.
No se puede definir una variable local con la palabra clave "static".

Variables de Instancia:
Alcance: Las variables de instancia se declaran dentro de una clase pero fuera de cualquier método o bloque. Cada objeto de la clase tiene su propia copia de estas variables.
Duración de vida: Las variables de instancia existen mientras el objeto al que pertenecen está en uso. Cuando se crea una instancia de la clase, se asignan valores iniciales a las variables de instancia. Permanecen en memoria mientras el objeto está vivo.
No se puede definir una variable local con la palabra clave "static".

Variables Estáticas (o variables de clase):
Alcance: Las variables estáticas también se declaran dentro de una clase, pero se etiquetan con la palabra clave static. Estas variables pertenecen a la clase en lugar de a objetos individuales, lo que significa que todas las instancias de la clase comparten la misma variable estática.
Duración de vida: Las variables estáticas existen mientras la clase está cargada en memoria. No están vinculadas a instancias específicas, por lo que su valor es compartido entre todas las instancias de la clase.

**Ejemplo:**
```java
public class EjemploUsoVariables {
    int variableDeInstancia; // variable de instancia
    static int variableEstatica; // variable estática

    public void ejemploMetodo() {
        int variableLocal = 42; // variable local
    }

    public static void main(String[] args) {
        EjemploUsoVariables objeto1 = new EjemploUsoVariables();
        objeto1.variableDeInstancia = 10;
        objeto1.variableEstatica = 100;

        EjemploUsoVariables objeto2 = new EjemploUsoVariables();
        objeto2.variableDeInstancia = 20;

        System.out.println(objeto1.variableDeInstancia); // Imprime 10
        System.out.println(objeto2.variableDeInstancia); // Imprime 20
        System.out.println(objeto1.variableEstatica);    // Imprime 100
        System.out.println(objeto2.variableEstatica);    // Imprime 100 (misma variable estática)
    }
}
```

## TIPOS DE DATOS:
Los tipos de datos especifican los diferentes tamaños y valores que se pueden almacenar en la variable. Los tipos de datos en Java se pueden dividir en dos partes:

- Tipos de datos primitivos:
* boolea: Se utiliza para almacenar sólo dos valores posibles: verdadero y falso.
byte: Es un entero de 8 bits. Su rango de valores se encuentra entre -128 y 127.
char: El char se utiliza para almacenar un solo carácter. El carácter debe estar entre comillas simples ''.
short: 
int 
long 
float 
double 

- Tipos de datos no primitivos : que incluyen clases, matrices e interfaces.




FUENTES - RECURSOS:
- https://roadmap.sh/java
- https://www.w3schools.com/java/
- https://www.javatpoint.com/java-tutorial
- https://www.udemy.com/course/master-completo-java-de-cero-a-experto/
- https://www.jetbrains.com/help/idea/getting-started.html
