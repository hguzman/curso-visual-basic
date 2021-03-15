# Condicionales 

Tal a como desde un principio hace alusión, se trata de un condicionamiento (condición) que 
se aplica a una instrucción. Las condicionales, son aquellas que nos permiten ejecutar
una instrucción, si  se cumple la condición que hemos establecido. 

En **VBC** hay diferentes estructuras de condicionales, cada una de ellas con funciones específicas, como lo presentamos a continuación.

## Condiciones:

Comencemos por:

### if
 
**if** o tambien conocida como **si**, se encarga de acreditar si se cumple la o las funciones establecidas y de 
acuerdo a ello, si lo establecido es verdadero, realiza algo; y si no lo es realiza otra acción. A continuación encontrarás 
la especificación de la estructura **if**, lo que la compone y su construcción básica.

* If = si
(*condición*) = Aquí estaría la condición que queremos que se cumpla, es decir:
   * 1 **=** igual a
   * 2 **<>** Desigual
   * 3 **<** Menor a 
   * 4 **>** Mayor a 
   * 5 **<=** Menor o igual a 
   * 6 **>=** Mayor o igual a
* then = Entonces...  es decir, lo que se va a hacer de acuerdo a 
* *instrucciones* = Aquí va la orden a realizar, a partir de lo que respecte el cumplimiento de la condición.
* End if = Es el cierre o conclusión después de haber cumplido las instrucciones establecidas. 
   
   * **representación**
   
   ```
   if (*condición*) then
        `*instrucción*
   End if
   ```
    
 ## Dependiendo de (Select case)
  **Select case**, en el lenguaje de programación, es una instrucción que le permite al usuario asignar, clasificar u organizar a partir 
 de una variable, sus posibles resultados. Esta instrucción es una alternativa al **If. Then. Else** y permite evaluar varias condiciones de manera mas formal u organizada.
 
  * **representación**
  La condición inicia con **Select case + Variable** y se cierra con **End select**
    ```
    Select case (variable)
         case 1
             (proceso del caso 1 *suma, resta, multiplicación, etc.)
         case 2
             (proceso del caso 2 *suma, resta, multiplicación, etc.)
         case 3
             (" " ")
          case ...
    End select
    ```
     
 **Ejemplo:**
  A continuación se presenta un programa que le pide al usuario registrar dos numeros y posterior a ello, plantea las opciones posibles al porceso, 1. Suma, 2. Resta, 3. multiplicación, 0. Salir del proceso. Seguidamente, se emplea la condición con los respectivos casos de acuerdo a la opción previamente establecida por el usuario (case 1, case 2, case 3). Finalmente, después de cerrarse la condición, se emitirá un mensaje que contenga la solución a la condición establecida.
 
 ```
  Sub casos()
    Do
        n1 = Int(InputBox("Registre numero"))
        n2 = Int(InputBox("Registre numero"))
        op = Int(InputBox("Seleccione una opcion: " & vbCrLf & "1. Suma" & vbCrLf & "2. Resta" & vbCrLf & "3. Multipliación" & vbCrLf & "0 .Salir"))
        
        Select Case op
            Case 1
                r = n1 + n2
            Case 2
                r = n1 - n2
            Case 3
                r = n1 * n2
        End Select
        MsgBox "Resultado" & r
        
    Loop Until (op = 0)
 End Sub
 ```
