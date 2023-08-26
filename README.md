# CONVERTIDOR_A_MEDIDAS
ES UN  CONVERTIDOR DE MEDIDAS DE CENTIMETROS A 5 MEDIDAS DIFERENTES 
```cpp
#include <iostream>

using namespace std;

int main() {
    double centimeters;
    std::cout << "Ingrese la longitud en centimetros: ";
    std::cin >> centimeters;

    int choice;
    std::cout << "Elija la unidad que quiere convertir:\n";
    std::cout << "1. Metros";
    std::cout << "2. Yardas";
    std::cout << "3. Varas";
    std::cout << "4. Pulgadas";
    std::cout << "5. Pies";
    std::cout << "Ingrese su elección: ";
    std::cin >> choice;

    double result;

    switch (choice) {
        case 1:
            result = centimeters /100.0;
            std::cout << result << " metros." << std::endl;
            break;
        case 2:
            result = centimeters / 91.44;
            std::cout << result << " yardas." << std::endl;
            break;
        case 3:
            result = centimeters / 83.8235;
            std::cout << result << " varas." << std::endl;
            break;
        case 4:
            result = centimeters / 2.54;
            std::cout << result << " pulgadas." << std::endl;
            break;
        case 5:
            result = centimeters / 30.48;
            std::cout << result << " pies." << std::endl;
            break;
        default:
            std::cout << "Opción inválida." << std::endl;
    }

    return 0;
}

    double result;

    switch (choice) {
        case 1:
            result = centimeters /100.0;
            std::cout << result << " metros." << std::endl;
            break;

        case 2:
            result = centimeters / 91.44;
            std::cout << result << " yardas." << std::endl;
            break;

        case 3:
            result = centimeters / 83.8235;
            std::cout << result << " varas." << std::endl;
            break;

        case 4:
            result = centimeters / 2.54;
            std::cout << result << " pulgadas." << std::endl;
            break;

        case 5:
            result = centimeters / 30.48;
            std::cout << result << " pies." << std::endl;
            break;

        default:
            std::cout << "Opción inválida." << std::endl;
    }

    return 0;
}
-------------------------------------------------------------------

```python
def main():
    centimeters = float(input("Ingrese la longitud en centimetros: "))
    
    print("Elija la unidad a la que desea convertir:")
    print("1. Metros")
    print("2. Yardas")
    print("3. Varas")
    print("4. Pulgadas")
    print("5. Pies")
    
    choice = int(input("Ingrese su elección: "))
    
    result = 0.0
    
    if choice == 1:
        result = centimeters / 100.0
        print(result, "metros.")
    elif choice == 2:
        result = centimeters / 91.44
        print(result, "yardas.")
    elif choice == 3:
        result = centimeters / 83.8235
        print(result, "varas.")
    elif choice == 4:
        result = centimeters / 2.54
        print(result, "pulgadas.")
    elif choice == 5:
        result = centimeters / 30.48
        print(result, "pies.")
    else:
        print("Opción no válida.")

if __name__ == "__main__":
    main()


-------------------------------------------------------------------

## Convertidor de Longitud en Pseudocódigo  

Definir `centimeters` y `result` como números reales.
Definir `choice` como número entero.
   
Escribir "Ingrese la longitud en centímetros: "
Leer `centimeters`
   
Escribir "Elija la unidad a la que desea convertir:"
   - 1. Metros
   - 2. Yardas
   - 3. Varas
   - 4. Pulgadas
   - 5. Pies
Escribir "Ingrese su elección: "
Leer `choice`
   
   Si `choice` es igual a 1 Entonces
     - `result` = `centimeters` * 0.01
     - Escribir `result`, " metros."
   
Sino Si `choice` es igual a 2 Entonces
     - `result` = `centimeters` * 0.0109361
     - Escribir `result`, " yardas."
   
Sino Si `choice` es igual a 3 Entonces
      - `result` = `centimeters` * 0.8359
      - Escribir `result`, " varas."
   
Sino Si `choice` es igual a 4 Entonces
      - `result` = `centimeters` * 0.393701
      - Escribir `result`, " pulgadas."
   
Sino Si `choice` es igual a 5 Entonces
      - `result` = `centimeters` * 0.0328084
      - Escribir `result`, " pies."
   
Sino
      - Escribir "Opción no válida."
   
Fin Si

Fin Algoritmo


