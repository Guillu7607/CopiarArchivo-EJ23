# Resumen
Este proyecto consiste en una aplicación de consola en Java diseñada para realizar la duplicación e infraestructura de volcado de archivos. El objetivo principal del ejercicio es aprender a canalizar flujos de entrada y salida de caracteres de forma simultánea, leyendo desde un archivo origen (FileReader) y escribiendo en un destino (FileWriter) mediante el uso de búferes intermedios para maximizar el rendimiento de la operación.

## Características
Doble Flujo con Búfer: Acopla BufferedReader y BufferedWriter de forma paralela, logrando que los ciclos de lectura y escritura en el disco duro se realicen en bloques de memoria interna en lugar de carácter por carácter.

Preservación de la Estructura Lineal: Utiliza el método .newLine() para asegurar que el archivo de destino mantenga exactamente los mismos saltos de línea y el formato del documento original.

Gestión de Recursos Dual Simétrica: Implementa la estructura try-with-resources declarando múltiples flujos separados por punto y coma (;). Java se encarga de cerrar ambos descriptores de archivos de manera automática en orden inverso a su apertura.
