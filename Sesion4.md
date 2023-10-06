## Actividad 4: Ejercicios de control de flujo con expresiones compuestas
- // Variables de tipo String
- String nombre = "Juan Pérez";
- String apellido = "González";
- String identificación = "1000000001";
- String correo = "juan.perez@ejemplo.com";
- String carrera = "Desarrollo de Software";
- String universidad = "Cesde";
- // Variable de tipo int
- int edad = 20;
- // Variable de tipo boolean
- boolean esActivo = true;
- boolean becado = false;
- // Variable de tipo char
- char género = 'M';
- // Variable de tipo double
- double promedio = 4.5;
- // Variable de tipo int
- int semestre = 2;

- Con la información anterior, implementa los siguientes ejercicios:

- Determinar si el estudiante es mayor de edad y tiene un estado activo.
- Determinar si el estudiante tiene una beca o una carrera relacionada con el desarrollo de software.
- Determinar si el estudiante está en el último semestre de su carrera y tiene un estado activo.
- Determinar si el estudiante tiene una carrera relacionada con el desarrollo de software y un promedio superior a 4.0.
- Mostrar toda la información del estudiante si está matriculado en el Cesde.
- Asignar una beca del 50% si el estudiante está matriculado en el Cesde, tiene un promedio superior a 4.0 y está activo.
- Determinar la cantidad de beca que recibe el estudiante según su promedio:
- 0.0 - 3.4: El estudiante no recibe beca.
- 3.5 - 3.9: El estudiante recibe una beca parcial del 25%.
- 4.0 - 4.4: El estudiante recibe una beca parcial del 50%.
- 4.5 - 5.0: El estudiante recibe una beca completa.

## Desarrollo 
public class LogicaEstructuraCondicional {

    public static void main(String[] args) {
        // Variables de tipo String
        String nombre = "Juan Pérez";
        String apellido = "González";
        String identificación = "1000000001";
        String correo = "juan.perez@ejemplo.com";
        String carrera = "Desarrollo de Software";
        String universidad = "Cesde";
// Variable de tipo int
        int edad = 20;
// Variable de tipo boolean
        boolean esActivo = true;
        boolean becado = false;
        boolean ultimoSemestre = true;
        boolean otraCarrera = true;
        boolean promedioMayor4 = true;
        boolean matriculado = true;
// Variable de tipo char
        char género = 'M';
// Variable de tipo double
        double promedio = 4.5;
// Variable de tipo int
        int semestre = 2;
       
        System.out.println("Ejercicio 1");
        if (edad >= 18 && esActivo){
            System.out.println("Es mayor de edad");
        }
       
        System.out.println("--------");
        System.out.println("Ejercicio 2");
       
        if (becado || otraCarrera){
            System.out.println("No es becado pero tiene una carrera relacionada con el desarrollo"
                    + "de software");
           
            System.out.println("-------");
            System.out.println("Ejercicio 3");
           
            if (esActivo && ultimoSemestre){
                System.out.println("El estudiante es activo pero no esta en ultimo semestre");
            }
           
            System.out.println("------");
            System.out.println("Ejercicio 4");
           
            if (otraCarrera && promedioMayor4){
                System.out.println("Tiene una Carrera relacionada con el desarrollo de software"
                        + "y un promedio mayor a 4.0");
            }
           
            System.out.println("-----");
            System.out.println("Ejercicio 5");
           
            if(universidad.equals("Cesde")){
                System.out.println(" Nombre " + nombre);

                System.out.println(" Apellido " + apellido);

                System.out.println(" Identificación " + identificación);

                System.out.println(" Correo " + correo);

                System.out.println(" Carrera " + carrera);

                System.out.println(" Edad " + edad);

                System.out.println("esActivo");

                System.out.println(" Género " + género);

                System.out.println(" Semestre " + semestre);
                
                System.out.println("Promedio 4.5");
            }
           
            System.out.println("--------");
            System.out.println("Ejercicio 6");
           
            if(matriculado && promedioMayor4 && esActivo){
                System.out.println("Obtiene una beca del 50%");
               
            }
           
            System.out.println("------");
            System.out.println("Ejercicio 7");
           
            if (promedio < 3.4){
                System.out.println("No recibe beca");
            }
            if (promedio >= 3.5){
                System.out.println("El estudiante recibe una beca parcial del 25%");
            }
            if (promedio >= 4.0){
                System.out.println("El estudiante recibe una beca del 50%");
            }
            if (promedio >= 4.5 ){
                System.out.println("Recibe una beca completa");
            }
           
            Manuela Orlas
            Alejandra Tamayo        
           
        }
    }
}