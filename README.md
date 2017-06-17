# caracteres

package caracteres;

import java.util.Scanner;

public class Caracteres {

    public static void main(String[] args) {
     
    Scanner entrada = new Scanner (System.in);
    
    System.out.println("Ingrese una palabra");
    String cadena = entrada.nextLine();
    int letra =0;
    char caracter;
    
    
        for (int i =0;i<letra;i++){
        caracter=(char) cadena.charAt(i);
            if (caracter == ' '){
                System.out.println();
            }else {
                if (letra%2==0){
                    if (Character.isUpperCase(caracter)){
                        System.out.println(caracter);
                     }else if (Character.isLowerCase(caracter)){
                         caracter=(char)(caracter-'a'+'A');
                         System.out.print(caracter);
                     }
            
                }else {
                    if (Character.isLowerCase(caracter)){
                        System.out.println(caracter);
                    }else if(Character.isUpperCase(caracter)){
                        caracter=(char)(caracter-'a'+'A');
                        System.out.println(caracter);
                    }
                }
                letra++;
            }
        }
    }
}
