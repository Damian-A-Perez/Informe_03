# Informe_03

TEMA: PRÁCTICA No. 3 Analisis de nodos

ESTUDIANTES:  MENESES JARRIN SANTIAGO JAVIER OSEJO CUESTA BRANDON DILLAN PEREZ CEDILLO DAMIAN ALEXANDER 
    
DOCENTE: DARWIN OMAR ALULEMA FLORES 
 
NRC:  8703

En esta pratica determinaremos el funcionamiento del analisis en los nodos respectivo utilizando conocimientos previos aplicados experimentalmente en un circuito mixto de resistencias con dos fuentes de pueder. Se tomara como herramienta un simulador para crear un circuito a escala y observar cual es su comportamiento con respecto al calculo y los analisis previamente establecidos usando la Ley de Corrientes de Kirchhoff

1° Plantamiento del problema 
	
 Determinar el valor de las corrientes en relacion a los voltajes en cada nodo usando la Ley de corrientes de Kirchhoff como base para el calculo analitico, tomando como referencia este termino debemos establecer la relacion de las corrientes totales que pasan por un nodo, teniendo en cuenta que toda corriente que entra tiene una corriente, como minimo, que saldra del mismo nodo, generando la ecuacion donde la suma de todas las corrientes que entran y salen del nodo en cuestion debe dar como resultado un cero

2°Objetivo de la practiva 
	
  Comprobar experimentalmente el Análisis de Nodos.
 
 2.1° Objetivos especificos 
 
2.1.1 Definir cuales seran los nodos exactos donde se realizaran los calculos
  
 2.1.2 Dibujar la trayectoria supuesta para las corrientes en cada malla
  
  2.1.3 Observar el comportamiento de las corrientes por cada malla y en cada resistencia que atravieza
  
3° Marco Teorico

Nodo.- 
  Un nodo es definido como un punto de union o interseccion donde se encuentran dos o mas elementos entre si, genereando una corriente de entrada y de salida en dicha instancia de conexión
   
![Ejemplo nodo](https://github.com/Damian-A-Perez/Informe_03/blob/master/Img/Nodo.jpg)

Metodo de tensiones nodales.-
En circuitos electricos, el analisis de nodos se efectua mediante el metodo de tensiones nodales, el cual consiste en el uso de la ley de kirchhoff de corrientes para poder determinar el valor de los voltajes de uno o mas nodos dentro de un solo circuito cerrado
Para este analicis se establece una ecuacion para cada nodo en cuestion, tomando en cuenta como unica condicion que al usar el metodo de la ley de kirchhoff de corrientes (LCK) la suma de todas las corrientes dentro de aquel nodo debe ser igual a cero. Estas corrientes deben estar escritas en funcion de la tension, debido que es nuestra incognita.
Esta analisis solo es posible cuando todos los nodos disponene de conductancia, en caso de que los elementos del circuito no dispongan de conductancia, se usaria una extension mas compleja del analisis de nodos, conocida como Analisis de nodos modificado.

![Corrientes de un nodo](https://github.com/Damian-A-Perez/Informe_03/blob/master/Img/Corrientes%20de%20un%20nodo.png)

Usando este metodo, obtendremos un sistema de ecuaciones a establecer el cual puede ser resulto analiticamente mediante algebra lineal. Para que dicho sistema de ecuaciones sea consistente en sus totalidad, debe existir una ecuacion por cada nodo del circuito, tomando en cuenta la definicion de nodo, en tal caso obtendremos un numero de ecuaciones equivalente al numero de incognitas encontradas, que en este caso sera el numero de voltajes de nodo en todo el circuito.

4° Material Y Equipo 

![Material y equipo](https://github.com/Damian-A-Perez/Informe_03/blob/master/Img/Material%20y%20equipo%20(2).png)

5° Procedimiento 

![circuito para analisis de nodos](https://github.com/Damian-A-Perez/Informe_03/blob/master/Img/Circuito%20para%20analisis%20de%20nodos.png)

Implemente el circuito que se presenta en la figura

Mida cada uno de los voltajes de nodo y anotelos a continuacion

| NODO   | RESULTADOS ANALITICOS | RESULTADOS EXPERIMENTALES | RESULTADOS SIMULADOS |
|  :---:   |  :---:                |            :---:          |       :---:          |
|    A   | 2.820[V]                |-                   | 2.820[V]           |
|    B    | 4.802[V]                |-                 |4.802[V]             |
|    C    | 0[V]                |-               |0[V]           |

![Circuito implementado](https://github.com/Damian-A-Perez/Informe_03/blob/master/Img/Simulador3.png)



6° Explicacion del codigo fuente

Para implementar correctamente un circuito dentro del simulado, en primera instancia debemos encontrar y seleccionar los elementos a utilizar en el circuito completo, colocar una fuente de poder en cada extremo del circuito, asegurandonos de que la conexion vaya por toda la placa y poder usar mas espacio para conectar elementos, asegurarse de que las resistencias sean del valor adecuado y estan conectados concorde al circuito solicitado, teniendo en consideracion que dentro de un protoboard los nodos se representan de manera vertical asegurandonos espacios para conectar adecuadamente un punto de union.
El circuito requiere dos fuentes de voltaje, una de 12 v, la cual administrara la corriente de entrada hacia la primera resistencia, la cual tiene un valor de 1.8kohm, la otra fuente de voltaje es el punto de llegada de la resitencia de 1.5Kohm la cual cierra el circuito el cual fue previamente simulado con cuidado teniendo en consideracion la conexion de cada uno de los elementos del mismos para un correcto funcionamiento. 


Cronograma:
![cronograma](https://github.com/Damian-A-Perez/Informe_03/blob/master/Img/L3I1.png)
  
