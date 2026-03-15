#include <iostream>

int main() {
    double a, b, c;

    // Lectura de  los datos
    std::cout << "Ingrese el valor de a: ";
    std::cin >> a;
    std::cout << "Ingrese el valor de b: ";
    std::cin >> b;
    std::cout << "Ingrese el valor de c: ";
    std::cin >> c;

    // Validación de división por cero
    // La fórmula R = ((a + 2b) * (c - b)) / (a - c)
    // El denominador es (a - c). Si a == c, el resultado es 0.
    if (a == c) {
        std::cout << "Division por cero" << std::endl;
    } else {
        // Cálculo de R con paréntesis explícados para asegurar la procedencia
        // Estructura: R = [ (a + (2 * b)) * (c - b) ] / (a - c)
        double R = ((a + (2 * b)) * (c - b)) / (a - c);

        // Salida con etiqueta clara
        std::cout << "R=" << R << std::endl;
    }

    return 0;
}
