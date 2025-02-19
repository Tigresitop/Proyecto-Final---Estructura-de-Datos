![image alt](https://github.com/Tigresitop/Proyecto-Final---Estructura-de-Datos/blob/c54cba920c12ee72e65ae6b24eb12f60a56becc6/images/logo-ups.jpg)

# Proyecto Final

- Carrera: Computación.
- Materia: Estructura de Datos.
- Fecha de entrega: 18/02/2025.
- Docente: Ing. Pablo Torres.
Integrantes:

◦ David Larriva [dlarrivac@est.ups.edu.ec](mailto:dlarriva@est.ups.edu.ec)

◦ John Tigre [jtigrec4@est.ups.edu.ec](mailto:jtigrec4@est.ups.edu.ec)

◦ Patricio Mora [pmashinkiash@est.ups.edu.ec](mailto:pmashinkiash@est.ups.edu.ec )

## Descripción del Problema

- El proyecto consiste en desarrollar una aplicación que permita simular y analizar el recorrido de un laberinto mediante algoritmos de búsqueda como BFS (Breadth-First Search), DFS (Depth-First Search), búsqueda recursiva y con memorización (Cache). 

- El sistema deberá permitir la configuración dinámica del tamaño del laberinto, la selección de celdas no transitables (obstáculos) y la elección de puntos de inicio y destino para la simulación.

- El objetivo principal del proyecto es encontrar la ruta más óptima entre dos puntos dentro del laberinto, respetando las restricciones de movimiento (puede desplazarse hacia arriba, abajo, izquierda o derecha) y evitando obstáculos que bloqueen el camino.

- Además, la aplicación debe ser capaz de comparar los tiempos de ejecución de los diferentes algoritmos para determinar cuál de ellos es el más eficiente en distintos escenarios de prueba.
___
## Propuesta de Solución

### Marco Teórico
#### 1. Teoría de Grafos
La teoría de grafos es un campo de estudio matemático que modela relaciones entre elementos mediante nodos (vértices) y conexiones (aristas). En este proyecto, el laberinto se representa como un grafo donde las celdas son nodos y sus conexiones representan caminos disponibles.

#### 2. Algoritmos de Búsqueda Implementados
- Programación Dinámica: Optimiza la búsqueda almacenando resultados previos para evitar cálculos redundantes.  
- BFS (Breadth-First Search): Explora el laberinto por niveles, asegurando encontrar el camino más corto.  
- DFS (Depth-First Search): Explora el laberinto en profundidad, siguiendo un camino hasta el final antes de retroceder.  
- Recursividad: Implementa la búsqueda de manera estructurada a través de llamadas recursivas.  

## Desarrollo
El proyecto fue desarrollado siguiendo el patrón MVC (Modelo-Vista-Controlador), facilitando la organización del código y su mantenimiento.

### Herramientas Utilizadas
◦ Lenguaje: Java  
◦ IDE: Visual Studio Code
◦ Framework: Java Swing para la interfaz gráfica  
◦ Control de Versiones: Git y GitHub  

### Explicación de las Clases
- Modelo (Model): Define la estructura del laberinto y los algoritmos implementados.  
- Vista (View): Contiene la interfaz gráfica para la interacción con el usuario.  
- Controlador (Controller): Administra la lógica del sistema y la comunicación entre el modelo y la vista.  

## Interfaz de Usuario (UI)
La aplicación cuenta con tres interfaces principales para configurar y ejecutar la simulación del laberinto.

### Interfaz 1: Configuración del Laberinto
 ◦ Permite ingresar el tamaño del laberinto (3x3 a 9x9).  
 ◦ Valida la entrada del usuario antes de continuar.  
 ◦ Botón "Siguiente" para avanzar a la siguiente configuración.  

### Interfaz 2: Selección de Obstáculos
◦ Muestra el laberinto visualmente.  
◦ Permite marcar hasta 4 celdas como obstáculos.  
◦ Botón "Siguiente" para continuar con la simulación.  

### Interfaz 3: Simulación del Laberinto
◦ Permite establecer punto de inicio y fin en la cuadrícula.  
◦ Visualiza la ruta generada por el algoritmo seleccionado.  
 ◦ Opción "Limpiar" para reiniciar la simulación.  
 ◦ Muestra tiempos de ejecución en nanosegundos para comparar eficiencia.  
 
En las siguientes imagenes se  mostrara el camino y tiempo que realiza cada uno de los algoritmos.
-Programación Dinamica: 

-BFS (Breadth-First Search):

-DFS (Depth-First Search): 

-Recursividad:


## Criterio por Estudiante

- Patricio Mora:  
  Patricio se enfocó en la implementación de los algoritmos de búsqueda, asegurándose de que cada uno (BFS, DFS, recursivo y memorización) funcionara correctamente y proporcionara resultados comparables en términos de eficiencia. A pesar de que los algoritmos operan de manera adecuada, identificó que el método recursivo presenta limitaciones de rendimiento en laberintos grandes, debido al alto consumo de memoria y la cantidad de llamadas recursivas necesarias. Como posible mejora, sugiere optimizar el manejo de memoria en este tipo de búsquedas o explorar alternativas que reduzcan el impacto en el rendimiento. Asimismo, considera que sería interesante incluir la opción de visualizar múltiples rutas óptimas en situaciones donde existan varias soluciones con el mismo costo.



- John Tigre:  
  John fue responsable del diseño e implementación de la interfaz gráfica, asegurando que la interacción del usuario con el sistema fuera intuitiva y funcional. Se logró desarrollar una interfaz que permite seleccionar obstáculos, definir los puntos de inicio y destino, y visualizar el recorrido generado por cada algoritmo. No obstante, considera que la experiencia de usuario podría mejorarse aún más, agregando elementos visuales como animaciones o un sistema de colores más intuitivo, que permitan una mejor comprensión del comportamiento de los algoritmos. También plantea que sería más práctico para el usuario poder marcar obstáculos directamente sobre la cuadrícula en lugar de ingresar coordenadas manualmente, lo que haría el proceso más dinámico y sencillo.

- David Larriva:  
  David se encargó principalmente de la estructura del código y la implementación del patrón Modelo-Vista-Controlador (MVC) para asegurar una correcta organización y separación de responsabilidades dentro del proyecto. Gracias a esto, se logró un código más modular y mantenible, facilitando su comprensión y futuras modificaciones. Sin embargo, considera que aún existen oportunidades de optimización, especialmente en la reducción de redundancias en ciertas clases y métodos. Además, sugiere que una posible mejora para versiones futuras del programa sería implementar una función de exportación que permita guardar y cargar laberintos previamente configurados, evitando así la necesidad de realizar la configuración manual en cada ejecución.
___

## Conclusión  

En la implementación de los diferentes métodos, se observaron los siguientes resultados:

- Método Recursivo: Funcional, pero su eficiencia disminuye en laberintos grandes por el alto consumo de memoria.  
- Programación Dinámica (Cache): Optimiza el rendimiento evitando cálculos redundantes.  
- BFS: El método más eficiente para encontrar la ruta más corta gracias a su exploración por niveles.  
- DFS: Puede ser más rápido en algunos casos, pero no siempre garantiza la mejor ruta y usa más memoria en laberintos grandes.  
___

##  Consideraciones  

- Patricio Mora:  
  Se logró implementar correctamente los algoritmos de búsqueda (BFS, DFS, Recursivo y Cache), pero se podría optimizar la gestión de memoria en búsquedas más complejas. Además, sería interesante añadir una funcionalidad para visualizar múltiples soluciones cuando existen varios caminos óptimos dentro del laberinto.  

- John Tigre:  
  La interfaz gráfica cumple con su función, pero podría mejorarse en términos de interactividad y diseño. Agregar animaciones o un sistema de colores más intuitivo ayudaría a que el usuario comprenda mejor el recorrido de cada algoritmo. También sería útil permitir la selección de obstáculos de una manera más visual, como haciendo clic en las celdas del laberinto en lugar de ingresar coordenadas manualmente.  

- David Larriva:  
  La estructura del código sigue el patrón MVC, lo cual mejora la organización, pero aún se pueden realizar optimizaciones. Sería útil reducir la cantidad de clases y mejorar la reutilización de código para evitar redundancias. Además, se podría implementar una funcionalidad de exportación para guardar los laberintos y resultados, lo que permitiría analizar diferentes escenarios sin necesidad de reconfigurar todo desde cero.
