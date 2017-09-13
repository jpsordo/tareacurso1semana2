# tareacurso1semana2
/*Tarea iOS Curso 1 Semana 2.

GEnerar una serie de números del cero al 100 con el 100 incluído e imprimirlos según las siguientes condiciones :

1.- Si es divisible entre 5 imprimir número y #BINGO!!! 2.- Si es par debe imprimir el número y PAR 3.- Si es impar debe imprimir número e IMPAR 4.- En el rango 30...40 imprimir número más #VIVASWIFT!!!

Se debe usar la interpolación de variables en la impresión.

Gracias por calificar.

PD : Los números los imprime una vez para que se logre una visualización más ordenada.
*/

import UIKit

var numero = 1...100

for resultado in numero {
    
    /* Variables para imprimir todo en la misma línea
     de número */
  
    var expresion1 : String = "          "
    var expresion2 : String = ""
    var expresion3 : String = ""
    
    if resultado % 5 == 0 {
        expresion1 = " #BINGO!!!"
        }
    
    if resultado % 2 == 0 {
        expresion2 = " PAR   "
        }
            
    if resultado % 2 != 0 {
        expresion2 = " IMPAR "
        }
                
    if resultado >= 30 && resultado <= 40 {
        expresion3 = "   #Viva SWIFT !!!"
    }
    
    if resultado < 10 {
        print("0\(resultado)\(expresion1)\(expresion2)\(expresion3)")
        
    }else{
        print("\(resultado)\(expresion1)\(expresion2)\(expresion3)")
    }
    
    

                        }

