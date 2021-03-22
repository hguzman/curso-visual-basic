# **¿que es una variable constante en programacion?**
  Una constante es una variable con un valor que no puede ser alterado durante la ejecución del programa. Tan solo se puede leer, no se puede modificar. Si en nuestro programa tenemos que usar el número Pi, este siempre va a ser el mismo, no va a cambiar, así que este por seguridad debería ser una constante para asegurarnos de que nunca va a cambiar

## **Ejemplos de constante**

  **c++**
    se usa la palabra clave const seguido del tipo de dato que queramos incluir o por medio del comando #define nombre_constante valor.
    **Ejemplo**
     **#define PI  3.1415926**
     **const tipo_de_dato nombre_de_la_constante = valor_de_la_constante;**

   **Pascal**
    En el lenguaje de programación Pascal es posible declarar constantes de cualquier tipo de dato utilizando (al igual que C++) la palabra reservada const.
    **Ejemplo**
     **const tipo_de_dato nombre_de_la_constante = valor_de_la_constante;**

    **C**
    las constantes se declaran con #define.
    **Ejemplo**
       **#define PI  3.1415926**

    **Java**
     se definen mediante el modificador final.
    **Ejemplo**
     **static final nombreConstante = valor;**
     **static final int DIAS_SEMANA = 7;**
