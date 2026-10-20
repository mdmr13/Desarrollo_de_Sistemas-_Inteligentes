
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
Actividad 3.3 
Preguntas
**1. Sección “How does machine learning work?”** El artículo menciona tres tipos de aprendizaje. Anótalos y escribe con tus palabras en qué se diferencian.

Aprendizaje supervisado: aprende a partir de datos que ya tienen respuestas correctas o etiquetas
Aprendizaje no supervisado: recibe datos sin respuestas previamente indicadas y busca patrones, semejanzas o grupos. 
Aprendizaje por refuerzo: aprende mediante la interacción con su entorno, recibiendo recompensas o penalizaciones según sus acciones

Osea Supervisado aprende con ejemplos con respuestas, No Supervisado descubriendo patrones por su cuenta y Por Refuerzo mediante las consecuencias de sus decisiones. 

**2. Sección “What is machine learning used for?”** Elige una aplicación (reconocimiento de imágenes, diagnóstico médico, conducción automática, texto y voz) y describe con las ideas de la clase de qué se trata: ¿cuál sería la tarea (T) y qué datos serían la experiencia (E)?

El Machine Learning puede analizar información medica para identificar patrones relacionados con enfermedades y ayudar a los médicos a detectar posibles problemas.

T: identificar si un paciente podría tener una enfermedad a partir de sus síntomas, laboratorios o estudios médico

E: conjunto de datos de pacientes anteriores, sus síntomas, resultados de análisis y diagnósticos confirmados 

**3. Sección “When to use machine learning?”** Según el artículo, ¿cuándo conviene usar ML en lugar de reglas tradicionales? Da un ejemplo de un problema donde NO convendría.
Cuando se tienen grandes cantidades de datos y es difícil encontrar patrones o hacer predicciones mediante reglas tradicionales

Cuando si conviene: detectar transacciones bancarias sospechosas porque los fraudes pueden presentar patrones diferentes y cambiar con el tiempo 

Cuando no conviene: calcular el total de una compra con precios fijos; es suficiente con multiplicar las cantidades por sus precios y sumar los resultados, no es necesario un modelo 

**4. Sección de aplicaciones, “Fraud detection” y “Anomaly detection”.** El artículo dice que en detección de anomalías los modelos no supervisados detectan irregularidades sin datos etiquetados como “normales”. ¿Por qué un enfoque no supervisado tiene sentido para detectar fraudes raros? ¿Qué problema tendría un modelo supervisado?

Tiene sentido porque pueden aparecer de formas nuevas que todavía no está registradas, el modelo puede aprender los patrones habituales de las transacciones y señalar las inusuales 

El modelo supervisado tendría el problema de depender de ejemplos previamente etiquetados como fraudulentos o legítimos, como los fraudes poco comunes, podría haber pocos ejemplos para entrenarlo y no aprendería a reconocerlos en modalidades que nunca ha visto

**5. Sección de aplicaciones, “Healthcare” o “Finance”.** Elige una. Escribe qué error de un modelo sería **peor**, el falso positivo o el falso negativo, y explica por qué.

En el ámbito de la salud, considero que el error más grave sería el falso negativo porque ocurre cuando el modelo indica que no hay una enfermedad cuando en realidad si la hay, esto podría retrasar el diagnóstico y el tratamiento necesario, poniendo en riesgo la salud del paciente.

También en el falso positivo, el modelo indica que se tiene una enfermedad cuando en realidad no es así, causando preocupación y pruebas medicas innecesarias pero aquí la gravedad dependería más de la enfermedad y sus circunstancias

**6. Sección “Machine learning examples by company”.** Elige un caso (Meta, Amazon). ¿Qué datos crees que usa el sistema? ¿Quién se beneficia y quién podría salir perjudicado (por ejemplo, por privacidad)?

Amazon: usa ML para recomendar productos segun intereses y compras de clientes

Podría utilizar: historial de compras, productos consultados, búsquedas de artículos agregados al carrito y compras de otros usuarios con intereses similares

Beneficia: a los clientes porque pueden encontrar productos de su interés fácilmente y a Amazon aumentando sus ventas 

Perjudica: a los usuarios cuya privacidad se vea afectada por la recopilación y análisis de sus datos de consumo, podrían recibir recomendaciones demasiado personalizadas o quedar expuestos a publicidad que influya sus decisiones 

**7. Lectura crítica.** Revisa el título y la sección de experiencia de la empresa. Escribe al menos dos cosas que te hagan dudar de la información y qué le pedirías al autor para confiar más. (Pista: ¿cuántos casos promete el título y cuántos hay? ¿qué cifras aparecen sin explicar cómo se midieron? ¿quién escribe el artículo y qué vende?)

El título promete 12 aplicaciones de Machine Learning pero algunas son muy parecidas entre ellas, le preguntaría al auto cómo las clasificó. 

Menciona cifras como que la precisión de los pronósticos llega al 80% y que se puede aumentar la retención de usuarios más del 30% pero no explica cómo obtuvo esos datos ni que datos fueron utilizados para medirlo, preguntaría por las fuentes que "respaldan" estas cifras

Como es de una empresa que ofrece servicios de tecnología, me hace pensar que podría estar destacando más las ventajas del Machine Learning que sus desventajas; buscaría fuentes independientes que confirmen lo que dice. 
