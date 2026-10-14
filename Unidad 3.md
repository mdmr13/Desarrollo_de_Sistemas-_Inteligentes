
Actividad 3.1 Algoritmos de búsqueda
1) Problemas de búsqueda: Son problemas en los que se busca encontrar una secuencia de acciones que permita llegar desde un estado inicial hasta un objetivo deseado
2) Espacios de estados: Es el conjunto de todos los estados posibles por los que se puede pasar al resolver un problema
3) Estado inicial: Es la situación o condición en la que se encuentra el problema antes de comenzar la búsqueda
4) Acciones: Son las operaciones o movimientos que un agente puede realizar para pasar de un estado a otro
5) Modelo de transición: Es la descripción de cómo cambia un estado cuando se realiza una acción determinada
6) Prueba de meta: Es el procedimiento que permite comprobar si un estado cumple con las condiciones necesarias para alcanzar el objetivo
7) Costo del camino: Es el valor total asociado a una secuencia de acciones desde el estado inicial hasta un estado determinado. Puede representar distancia, tiempo, dinero o recursos utilizados 
8) Solución: Es una secuencia de acciones que permite llegar desde el estado inicial hasta un estado que cumple con el objetivo del problema
9) Frontera: Es el conjunto de nodos generados durante la búsqueda que están pendientes de ser explorados
10) Nodo: Es una representación de un estado dentro del árbol de búsqueda, que contiene información como el estado, la acción realizada para llegar a él, su nodo padre y el costo acumulado del camino 
11) Agente de resolución de problemas: Es un agente inteligente que identifica un objetivo, formula un problema y utiliza algoritmos de búsqueda para encontrar una secuencia de acciones que permita alcanzar dicho objetivo

Sistemas de búsqueda (ciega)
1) Búsqueda no informada (ciega): Es un método de búsqueda que explora los estados posibles sin utilizar información adicional sobre qué tan cerca se encuentran del objetivo
2) Búsqueda en amplitud: Es un algoritmo que explora primero todos los nodos de un mismo nivel antes de avanzar al siguiente. Utiliza una cola para organizar los nodos pendientes
3) Búsqueda en profundidad: Es un algoritmo que explora una rama hasta donde sea posible antes de regresar y explorar otras ramas. Utiliza una pila o un mecanismo de retroceso
4) Búsqueda de costo uniforme: Es un algoritmo que expande primero el nodo con el menor costo acumulado desde el estado inicial. Permite encontrar una solución de costo mínimo si se cumplen las condiciones necesarias
5) Cola: Es una estructura de datos que sigue el principio FIFO (First In, First Out), es decir, el primer elemento en entrar es el primero en salir. Se utiliza en la búsqueda en amplitud
6) Pila: Es una estructura de datos que sigue el principio LIFO (Last In, First Out), es decir, el último elemento en entrar es el primero en salir. Se utiliza en la búsqueda en profundidad
7) Completitud: Es la propiedad de un algoritmo que garantiza encontrar una solución si existe, siempre que se cumplan determinadas condiciones
8) Optimalidad: Es la propiedad de un algoritmo que garantiza encontrar la mejor solución posible, generalmente la de menor costo
9) Complejidad en tiempo: Es la cantidad de tiempo o de operaciones que necesita un algoritmo para encontrar una solución, según el tamaño del problema
10) Complejidad en espacio: Es la cantidad de memoria que necesita un algoritmo para almacenar los nodos y la información durante el proceso de búsqueda

![[Pasted image 20261008181203.png]]


Busca primero las rutas más cercanas y luego las más lejanas, si cada pasito cuesta lo mismo, encuentra el camino con menos pasos


![[Pasted image 20261008181320.png]]

Busca el camino que cueste menos recorrer, si todos los movimientos cuestan lo mismo, va a buscar un camino con la menor cantidad de pasos

Actividad 3.2 
Compara en la página dos algoritmos (A*) y uno ciego. Contestar las preguntas: 
Qué longitud tiene cada algoritmo? El primero (Manhattan) 16 y el segundo (Ciego) también
Cuánto tiempo se tardo cada algoritmo? El Manhattan 0.4000ms y el Ciego 1.6000
Qué diferencia observas? El Manhattan es más rápido 

![[Pasted image 20261014155910.png]]
![[Pasted image 20261014155926.png]] 