# **¿Que es una variable acumuladora en programación?**
  Un acumulador es una variable numérica que permite ir acumulando operaciones. Me permite ir haciendo operaciones parciales. Un acumulador:

  ## **Ejemplo**
    - Se inicializa a un valor inicial según la operación que se va a acumular: a 0 si es una suma ó a 1 si es un producto.
    - Se acumula un valor intermedio.
        acum <- acum + num;

        Introducir 5 número y sumar los números pares.

          Proceso SumarPares
	           Definir var,suma,num como Entero;
	           suma<-0;
	           Para var<-1 Hasta 5 Hacer
		           Escribir sin saltar "Dime un número:";
		           Leer num;
		           Si num % 2 = 0 Entonces
			            suma<-suma+num;
		           FinSi
	           FinPara
	           Escribir "La suma de los números pares es:",suma;
         FinProceso
