package DIAGNOSTICO;
import java.util.Scanner;
public class Diagnostico {

    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        //Se declaran las variables a ocupar, en este caso n para las filas y m para las columnas
        int n, m;
        //Punto para que el usuario coloque la matriz 
        System.out.print("Ingresa el número de filas: ");
        n = in.nextInt();
        System.out.print("Ingresa el número de columnas: ");
        m = in.nextInt();
        //Con este ciclo se cuenta cada fila y columna para colocar los *
        for(int i=0;i<n;i++){ 
            //Esta linea coloca cada *
            for(int j=0;j<m;j++){
                System.out.print("*");
            }
            System.out.println(""); //Se induce un sato de linea
            m-=1; //Aqui se elimina un * por cada una de las filas para cada ciclo diferente
            //NOTA solo coloque hasta la instruccion 2 por que las demas no supe como hacerlas
        }        
    }
}
