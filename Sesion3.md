## Actividad 3: Ejercicios de operaciones básicas en Java.
- Suma y multiplicación: Escribe un programa que solicite al usuario dos números enteros y luego imprima la suma y multiplicación de esos números.

- Resta y división: Escribe un programa que tome dos números enteros ingresados por el usuario y calcule la resta y división de esos números.

- Operaciones combinadas: Escribe un programa que solicite al usuario tres números enteros y realice las siguientes operaciones: suma de los tres números, multiplicación del primer número por el segundo y división del resultado entre el tercer número.

- Operaciones con decimales: Escribe un programa que solicite al usuario dos números decimales y realice las siguientes operaciones: suma, resta, multiplicación y división.

- Incremento y decremento: Escribe un programa que declare una variable entera y la inicialice con un valor. Luego, incrementa su valor en 1 y muestra el resultado. Después, decrementa su valor en 1 y muestra el resultado nuevamente.

- Operador de asignación compuesta: Escribe un programa que declare una variable entera y la inicialice con un valor. Utiliza el operador de asignación compuesta para sumar 5 a la variable y luego mostrar su valor.

- Operadores lógicos: Escribe un programa que tome dos valores booleanos ingresados por el usuario y muestre el resultado de las operaciones lógicas AND, OR y NOT entre esos valores.

- Operador ternario: Escribe un programa que tome un número entero ingresado por el usuario y utilice el operador ternario para determinar si el número es positivo o negativo. Luego, muestra el resultado en la salida.

## Desarrollo 
### EJERCICIO 1 

public class LogicaProgramacion {
   public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.println("Ingrese un numero");
        int num1 = input.nextInt();
       
        System.out.println("Ingrese otro numero");
        int num2 = input.nextInt();
       
        int suma = num1 + num2;
        int multi = num1 * num2;
       
        System.out.println(" El resultado de la suma es: "+suma);
        System.out.println(" El resultado de la multi es: "+multi);      
    }
}

### EJERCICIO 2 
public class LogicaProgramacion {
   public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.println("Ingrese un numero");
        int num1 = input.nextInt();
       
        System.out.println("Ingrese otro numero");
        int num2 = input.nextInt();
       
        int resta = num1 - num2;
        int division = num1 / num2;
       
        System.out.println(" El resultado de la resta es: "+resta);
        System.out.println(" El resultado de la division es: "+division);   
    }
}

### EJERCICIO 3 
public class LogicaProgramacion {
   public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.println("Ingrese un numero");
        int num1 = input.nextInt();
       
        System.out.println("Ingrese otro numero");
        int num2 = input.nextInt();
       
        System.out.println("Ingrese otro numero");
        int num3 = input.nextInt();
       
        int suma = num1+ num2+ num3;
        int multi = num1 * num2;
        int division = multi / num3;
       
        System.out.println(" El resultado de los tres numeros es: "+suma);
        System.out.println(" El resultado de los numeros de la multiplicacion es: "+multi);
        System.out.println(" El resultado dela division del tercer numero es:" +division);
    }
}

### EJERCICIO 4 
public class LogicaProgramacion {
   public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Ingrese un número entero: ");
        int num = input.nextInt();
        int i= 0;
        int mult;

        while (i <= 10) {
            mult = num * i;
            System.out.println(num+" X "+i+" = "+mult);
            i++;
        }

        input.close();
    }
}

### EJERCICIO 5 
public class LogicaProgramacion {
   public static void main(String[] args) {
      int num = 5;
      num +=1;
      System.out.println(" Incremento :"+num);
      num -=1;
      System.out.println(" Decremento :"+num);
    }
}

### EJERCICIO 6
public class LogicaProgramacion {
   public static void main(String[] args) {
      int num = 10;
      num += 5;
      System.out.println(num);
    }
}
