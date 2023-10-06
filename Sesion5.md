## Actividad 5: Ejercicios de bucles
- Resolver los siguientes ejercicios:

## Ejercicios - while
- Pedir al usuario que ingrese un número y mostrar su tabla de multiplicar hasta el número 10.
- Pedir al usuario que ingrese una cadena de caracteres y contar la cantidad de caracteres que son números.

## Ejercicios - do while
- Escribe un programa en Java que imprima los números del 1 al 100, pero que se detenga si el usuario introduce un número negativo.
- Escribe un programa en Java que pida al usuario un número entero e imprima la tabla de multiplicar de ese número, pero que se detenga si el usuario introduce el número 0.

## Ejercicios - for
- Imprimir los números impares del 1 al 50.
- Imprimir los números primos del 1 al 100.

## Desarrollo 
## ESTRUCTURA WHILE
public class EstructuraRepetitivas {

public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.println(" Ingrese un numero entero");

        int numero = input.nextInt();

        int i = 0;

        int mult;
       
        while (i <= 10){
            mult = numero * i;
            System.out.println(numero+ " x "+i+"= "+mult);
            i++;
                   
        }
    }
}

## ESTRUCTURA WHILE
public static void main(String[] args) {
        Scanner Scanner = new Scanner(System.in);
       
        System.out.println(" Igrese una cadena de caracteres ");
        String cadena = Scanner.nextLine();
       
        int i = 0;
        int contadorNumero = 0;
       
        while (i < cadena.length()){
            char caracter  = cadena.charAt(i);
            if (caracter == '1' || caracter == '2' || caracter == '3' || caracter == '4' || caracter == '5' ||
             caracter == '6' caracter == '7'|| caracter == '8' || caracter == '9'){
            contadorNumero++;
        }
        i++;
       
        System.out.println(" La cadena ingresada contiene "+contadorNumero + " Numeros");
        }
       
    }



 ## DO WHILE 
public class EstructuraRepetitivas

public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
       
     int num ;
     
     do{
         System.out.println(" Ingrese un numero(Ingrese un numero negativo para detener ):");

         num = input.nextInt();
         
         while (num >= 0 && num <= 99){

             num += 1;

             System.out.println(" Numero :"+ num);
             
     
     } while (num >=0);
     System.out.println(" Termina el programa ");
     
    }
}

## DO WHILE 
public class EstructuraRepetitivas {

public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        int num;
        int i =0;
       
        do{
            System.out.println(" Ingrese un numero entero ( 0 para detenerse)");
            num = input.nextInt();
           
            if (num != 0){
                System.out.println(" Tabla de multiplicar del "+num+" :");
               
                while (i <=10){
                    int resultado = num *i;
                    System.out.println(num+"x"+i+" = "+resultado);
                    i++;
                }
                i=0;
            }
           
        } while ( num != 0);
        System.out.println("Termina el programa ");
     
    }
}

## FOR
public class EstructuraRepetitivas {

public static void main(String[] args) {

        for(int num = 1; num <= 50; num+=2){

            System.out.println(num);
        }
       
     
    }
}

## FOR
public class EstructuraRepetitivas {

public static void main(String[] args) {

        boolean primo;

        System.out.println(" Son numeros primos del 1 al 100 : /n");
       
        for (int num= 2; num <=100; num ++){

            primo= true;

            for(int i = num - 1; i > 1; i--){

                if (num % i == 0){

                    primo= false;

                    break;
                }
            }
            if (primo){
                
                System.out.println(num);
            }
        }
       
     
    }
}