
# LABORATORIO # 03

TEMA: Análisis de nodos
## 1. OBJETIVOS

**1,1.- GENERAL** 

* Comprobar experimentalmente el Análisis de Nodos. 

**1,2.-ESPECÍFICOS**

* Examinar el funcionamiento de un circuito mixto con 2 fuentes de voltaje.

* Comparar los valores medidos con los valores calculados en el circuito y establecer el porcentaje de error resultante.

* Aplicar el uso de las leyes de voltaje de Kirchhoff  para el análisis de mallas.


## 2. PLANTEAMIENTO DEL PROBLEMA

Este proyecto consistió en la implementación de un circuito electrónico virtual en un programa online denominado Tinkercad con la finalidad de experimentar una simulación del circuito donde es posible aplicar el Análisis de nodos. 

Se procede a realizar ensamblaje   del circuito con resistencias en serie y paralelo de diferentes valores para que estas formen mallas con el fin de poder realizar su análisis midiendo las corrientes de cada malla del circuito.


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


## 4. DIAGRAMAS

Para este laboratorio se utilizó un circuito mixto en donde podemos diferenciar que se encuentra constituido por 3 mallas.

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

| CORRIENTE | MEDIDO | CALCULADO  |
|----------|------|-------|
| I1 (A) | 0.01145 A | 0.0115 A|
| I2 (A) | 0.00285 A| 0.00285 A|
| I3 (A) | 0.00049 A | 0.000488 A |



- CÁLCULO DEL ERROR DE LA CORRIENTE

∑(Corriente calculado)= (0.0115 + 0.00285 + 0.000488) A

∑(Corriente calculado)=  0.01484 A

∑(Corriente medido)= (0.01145 + 0.00285 + 0.00049) A

∑(Corriente medido)= 0.01479 A 

%error=((Valor teórico-Valor medido)/Valor teórico)* 100

%error=((0.01484 A - 0.01479 A)/ 0.01484 A)* 100

%error= 0.34 % 

Como podemos observar los valores de cada corriente medida en las tres mallas con analisís de mallas son muy parecidos a los valores cálculados con el Tinkercad, ya que el porcentaje de error de la corriente es menor al 1%.

Habiendo simulado y creado el circuito, se observa que las corrientes con valores teóricos y los prácticos son semejantes, dando a conocer el funcionamiento del método de análisis de malla.

Conluimos generalmente que hay una pequeña diferencia entre los valores medidos y calculados, se podría dar por dos razones : al momento de calcular con el multímetro los valores, intervienen las tolerancias de las resistencias, y esto podría afectar a los valores obtenidos; mientras que en los valores medidos intervien la falta de utilización de todos los decimales,  lo cual afecta los valores obtenemos. 



## 11. RECOMENDACIONES

Recomendamos el asegurarse del correcto cálculo de los valores de manera clara y ordenada, de lo contrario, tendríamos un % de error excesivo. Es muy importante asignar una corriente de malla a cada malla (sentido cualquiera) y asignar una polarización a cada elemento del circuito.

Así mismo se recomienda cerciorarse de que la implementación de circuito este correctamente elaborado tal como está planteado.
Para terminar podemos sugerir utilizar de manera adecuada en serie el uso del multímetro para el cálculo de las corrientes.


## 12. CRONOGRAMA

![](https://github.com/BriandaLema/Laboratorio2/blob/master/img/Cronograma.png)

https://trello.com/b/0MUzNNnz/lab-2

## 13. BIBLIOGRAFÍA

* Antony, G. G. (26 de Julio de 2013). PANAMAHITEK. Obtenido de http://panamahitek.com/ley-de-los-voltajes-de-kirchhoff-metodo-de-mallas/#:~:text=En%20un%20circuito%20el%C3%A9ctrico%2C%20una,formadas%20por%204%20caminos%20cerrados.&text=Si%20multiplicamos%20las%20corrientes%20de,el%20total%20debe%20ser%20cero.

* Willi, M. (s.f.). KHAN ACADEMY. Obtenido de https://es.khanacademy.org/science/electrical-engineering/ee-circuit-analysis-topic/ee-dc-circuit-analysis/a/ee-mesh-current-method



## 14.- ANEXOS
https://github.com/BriandaLema/Laboratorio2/blob/master/ANEXOS/ANEXOS.pdf
