
# LABORATORIO # 03

TEMA: Análisis de nodos
## 1. OBJETIVOS

**1,1.- GENERAL** 

* Comprobar experimentalmente el Análisis de Nodos. 

**1,2.-ESPECÍFICOS**

* Aplicar el uso de las leyes de voltaje de Kirchhoff  para el análisis de nodos.

* Examinar el funcionamiento de un circuito mixto con 2 fuentes de voltaje.

* Comparar los valores medidos con los valores calculados en el circuito y establecer el porcentaje de error resultante.



## 2. PLANTEAMIENTO DEL PROBLEMA

Este laboratorio consistió en la implementació de un circuito mixto en un programa online denominado Tinkercad con la finalidad de experimentar una simulación del circuito donde es posible aplicar el Análisis de nodos basado en las Leyes de Kirchhoff. 

Se procede a acoplar y ensamblar el circuito con resistencias en serie y paralelo de diferentes valores para que estas forme el circuito en el cuál se pudo medir el valor de los voltajes pertenecientes a cada resistencia a traves de cada una de las intencidades que interfienen en distintos nodos del circuito.

## 3. MARCO TEÓRICO 

**NODO**

Un nodo es un punto donde se cruzan dos o más elementos de un circuito eléctrico , ya sea este elemento una fuente de voltaje, corriente, resistencias, etc. 

Ejemplo:

![](https://github.com/BriandaLema/Laboratorio3/blob/master/IMG/Ejemplo.png)

Este circuito tiene cuatro nodos : A, B, C y D. Tenemos que tomar en cuenta que los quiebres de las líneas no constituyen necesariamente nodos.

**ANÁLISIS DE NODOS**

![](https://github.com/BriandaLema/Laboratorio3/blob/master/IMG/Nodos.png)

En primer lugar, se establecen los nodos. En este caso, existen 6 nodos:

* Entre la fuente V1 de la izquierda y la resistencia 1.

* Entre las resistencias R1, R2 y R3. 

* Entre las resistencias R3, R4 y R5. 

* Entre las resistencias R5, R6 y R7.

* Entre la fuente V2 de la derecha y la resistencia R7. 

* Entre V1, R2, R4, R6 y V2.

En segundo lugar, se elige un nodo como referencia, en este caso se elegirá el nodo 0 como referencia. Para encontrar los voltajes en los nodos 2, 3 y 4 utilizamos la Ley de las Corrientes de Kirchhoff la cual propone que la sumatoria de las corrientes que entran a un nodo es igual a la sumatoria de las corrientes que salen del mismo:

∑ corrientes de entrada = ∑ corrientes de salida
 
Y para saber las corrientes hacemos uso de la ley de Ohm:

I=V/R


**Análisis en el nodo 2**

![](https://github.com/BriandaLema/Laboratorio3/blob/master/IMG/Nodo%202.png)

La única corriente que entra al nodo es la que viene de la fuente y la corriente que pasa por R2 y por R3 salen del nodo.

![](https://github.com/BriandaLema/Laboratorio3/blob/master/IMG/C%C3%A1lculo.png)

Se asume que los 10 voltios de la fuente es mayor al voltaje en el nodo 2 ya que se produce una caída de voltaje en la resistencia. Las corrientes que salen serán la corriente que va del nodo 2 al nodo 3 y las que van del nodo 2 a tierra. Se asume que el voltaje 2 es mayor que el voltaje en el nodo 3.  El voltaje en tierra es cero voltios. 
Al final simplificamos la ecuación e igualamos la ecuación a un término independiente:

V2/240 -  V3/ 240  +  V2/ 220  +  V2/310  =  1/31

Realizamos el mismo procedimiento en los siguientes nodos y obtendremos una serie de ecuaciones donde combinando y reordenando los términos  podremos resolverlos mediante matrices , y así obtener el voltaje en cada uno de los nodos. 

## 4. DIAGRAMAS

Para este laboratorio se utilizó un circuito mixto en donde podemos diferenciar que existen 5 nodos:

- Entre la fuente V1 de la izquierda y la resistencia 1.

- Entre las resistencias R1, R2 y R3. 

- Entre las resistencias R3, R4 y R5. 

- Entre la fuente V2 de la derecha y la resistencia R5. 

- Entre V1, R2, R4 y V2.

![](https://github.com/BriandaLema/Laboratorio3/blob/master/IMG/Laboratorio%203.png)

## 5. LISTA DE COMPONENTES

| CANTIDAD| ELEMENTO |
| ------- | -------------|
| 2       | Fuente de Voltaje C.D.  |
| 1       | Multímetro digital  |
| 1       | Resistor de 470 Ω   |
| 1       | Resistor de 3.9 kΩ   |
| 1       | Resistor de 1.5 kΩ|
| 1       | Resistor de 1.8 kΩ|
| 1       | Resistor de 2.2 kΩ|
| 1       | Protoboard                    |

## 6. MAPA DE VARIABLES 

Variables eléctricas: 
* Voltaje
* Resistores

## 7. EXPLICACIÓN CÓDIGO DE FUENTE

Para este laboratorio utilizamos el simulador de Tinkercad , el cual es un sofware de diseño de circuitos, en este dispositivo encontramos una gama alta de componentes electrónicos que se utilizan para la creación de circuitos y simular su funcionamiento.
Tinkercad funciona directamente en un navegador web moderno por lo cual una conexión a internet es fundamental para la utilización de esta fuente. 
El mismo programa nos guía y asesora acerca de lo que realizamos, por lo cual la utilizacion de esta fuente es muy práctica si tienes un conocimiento básico sobre circuitos eléctricos.Una herramienta característica de Tinkercad es quemientras la simulación está en marcha podemos ir modificando las variables de cada elemento y ver los cambios en el momento. También podemos obtener una lista con los materiales empleado  que nos sirvio para realizar las fichas técnicas.



## 8. DESCRIPCIÓN DE PRERREQUISITOS Y CONFIGURACIÓN

Fundamentalmente los prerrequisitos que requiere este laboratorio sería: un dispositivo tegnológico (sea un teléfono, una pc, un tableta, entre otras); pues trabajamos en un simulador online, nuestro segundo requisito es acceso a internet y finalmente tener conocimientos básicos sobre las leyes aplicadas, los componentes, elementos y variables que se utiliza para la creación del circuito.


## 9.APORTACIONES

Para complementar la correcta cuantificacion de valores calculados y valores medidos se utilizo una aplicación más denominada Multisim, que es un programa que se debe instalar en un sistema inteligente para poder hacer una grafica y simulación de un circuito.

## 10. CONCLUSIONES

**ANÁLISIS DE RESULTADOS Y CÁLCULO DEL ERROR**

ANÁLISIS DE NODOS

| NODO | MEDIDO| CALCULADO |
|----------|------|-------|
| 1 | 9.1801 V | 9.18 V|
| 2 | 2.8199 V | 2.82 V|
| 3 | -1.9817 V | -1.98 V|
| 4 | 4.8016 V | 4.8 V|
| 5 | -3.1984 V | -3.2 V|



- CÁLCULO DEL ERROR DE LA CORRIENTE

∑(Voltaje calculado)= (9.18 + 2.82 -1.98 + 4.8 -3.2 ) V

∑(Corriente calculado)= 11.62 V 

∑(Corriente medido)= (9.1801 + 2.8199 -1.9817 + 4.8016 - 3.1984) V

∑(Corriente medido)= 11.6215 V

%error=((Valor medido - Valor calculado)/Valor medido)* 100

%error=(( 11.6215 V- 11.62 V)/11.6215 V )* 100

%error=  0.013%

Como podemos observar los valores de cada voltaje medido en los nodos son muy parecidos a los valores cálculados con el Tinkercad, ya que el porcentaje de error de la corriente es menor al 1%.

Despues de crear el circuito podemos denotarque los voltajes en valores teóricos y en los prácticos son semejantes, dando a conocer el funcionamiento del método de análisis de nodos.

Conluimos generalmente que hay una pequeña diferencia entre los valores medidos y calculados, se podría dar por dos razones : al momento de calcular con el multímetro los valores, intervienen las tolerancias de las resistencias, y esto podría afectar a los valores calculados; mientras que en los valores medidos intervien la falta de utilización de todos los decimales,  lo cual afecta los resultados.



## 11. RECOMENDACIONES

Recomendamos el asegurarse del correcto cálculo de los valores de manera clara y ordenada, de lo contrario, tendríamos un % de error excesivo.

Así mismo se recomienda cerciorarse de que la implementación de circuito este correctamente elaborado tal como está planteado.
Para terminar podemos sugerir utilizar de manera adecuada en paralelo el uso del multímetro para el cálculo de los voltajes.


## 12. CRONOGRAMA

![](https://github.com/BriandaLema/Laboratorio3/blob/master/IMG/Cronograma%20lab%203.png)

https://trello.com/b/0H6PFJ5Y/lab-3

## 13. BIBLIOGRAFÍA

* ANTHONY, G. G. (26 de 07 de 2013). PANAMAHITEK. Obtenido de http://panamahitek.com/ley-de-las-corrientes-de-kirchhoff-metodo-de-nodos/

* JOSÉ, S. G. (2009). FUNDAMENTOS DE CIRCUITOS. Bogotá : Ediciones Uniandes.

* THOMAS, L. F. (2007). PRINCIPIOS DE CIRCUITOS ELÉCTRICOS. MÉXICO: Pearson Educación de México, S.A. de C.V.

## 14.- ANEXOS
https://github.com/BriandaLema/Laboratorio3/blob/master/Anexos/Anexos.pdf
